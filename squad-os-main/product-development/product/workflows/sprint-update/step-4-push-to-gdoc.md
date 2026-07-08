# Step 4: Push to Google Doc (optional)

## Goal

Auto-push the compiled sprint update to a shared Google Doc using the Google
Workspace MCP, so the shared doc stays in sync with the source markdown. Skip this
step if you'd rather transfer manually.

> Replace `<your-google-workspace-email>` and `<DOC_ID>` with real values (store
> the doc ID in the workflow config once you pick a standing doc).

---

## Process

### 1. Read the compiled output file
Read `output/YYYY-MM-DD-sprint-update.md`. Verify all sections are present:
- What We Shipped / Are Building (Step 1)
- Metrics Snapshot (Step 2)
- Next Steps (Step 3)

If a section is missing, stop and flag to the PM before pushing.

### 2. Locate the target Google Doc
```
mcp__google_workspace__search_docs({
  user_google_email: "<your-google-workspace-email>",
  query: "Marketplace Experience Sprint Update"
})
```

### 3. Prepare content for Google Docs
- Preserve heading hierarchy (H1 → Title, H2 → Heading 2, H3 → Heading 3)
- Convert markdown tables to Google Docs tables
- Preserve bold/italic/quote formatting and links

### 4. Push
**Option A — append to a rolling doc (default):** inspect structure, then insert the new update at the top.
```
mcp__google_workspace__inspect_doc_structure({ user_google_email: "<your-google-workspace-email>", document_id: "<DOC_ID>" })
mcp__google_workspace__modify_doc_text({ user_google_email: "<your-google-workspace-email>", document_id: "<DOC_ID>", start_index: <insertion_point>, text: "<formatted_content>" })
```
**Option B — new doc per cycle:**
```
mcp__google_workspace__create_doc({ user_google_email: "<your-google-workspace-email>", title: "Marketplace Sprint Update - YYYY-MM-DD", content: "<full_content>" })
```

### 5. Apply formatting
Batch-apply heading/format operations after inserting raw text (`mcp__google_workspace__batch_update_doc`).

### 6. Share link
Retrieve and present the doc link (`mcp__google_workspace__get_drive_shareable_link`), then tell the PM it's ready for Step 5.

---

## Error handling

| Scenario | Action |
|----------|--------|
| Doc not found | Search Drive, ask PM for doc ID |
| Auth failure | Prompt `mcp__google_workspace__start_google_auth` and retry |
| Content too large | Split into section-by-section inserts |
| Formatting fails | Push raw text first, note issues for PM to fix |

## Notes
- The markdown file remains the source of truth; the Google Doc is a distribution copy.
- Tables are the most fragile part of markdown→Docs conversion; verify the push by reading back the first lines.
