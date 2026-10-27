[README.md](https://github.com/user-attachments/files/34043045/README.md)
# Engage–Design · Collaborative annotated bibliography

This website is populated from `ED-Annotated bibliography (1).docx`, with **71 bibliography entries**, **4 source sections**, and the six thematic definitions from the original document. Nothing here is a fictional sample. The original citations, hashtags and annotations are preserved in the exported spreadsheet. The title, author and year columns were automatically extracted to support search and display, and should be reviewed before public publication.

## What's included

- `index.html` - a complete, self-contained, searchable public-facing website. Double-click it to preview. Its 71 entries are embedded directly, so it works even without a web server or Google account.
- `bibliography-template.csv` - importable to Google Sheets; contains the editable source bibliography.
- `bibliography-data.json` - structured copy of the bibliography and tag definitions for backup or further design.
- `review-notes.md` - import notes and items worth checking before public release.

## Collaborate with a small editorial group

1. Go to Google Drive, create a Google Sheet, then choose **File > Import > Upload** and import `bibliography-template.csv`.
2. Invite trusted collaborators using **Share** and grant **Editor** permissions to their individual accounts. Do not select "Anyone with the link can edit." Use one reading per row. Multiple topics can be entered separated by semicolons.
3. The existing rows can be edited; new bibliography items can be appended. Columns are `title`, `authors`, `year`, `citation`, `tags`, `annotation`, `article_url`, `file_url`, `section`, and `editor_note`. The bibliography appears publicly in the website while editing takes place in Google Sheets.
4. To allow the website to load live data, in the Google Sheet choose **File > Share > Publish to web** (if enabled for your account), select only the bibliography tab and CSV as the publishing format. Copy its public CSV URL.
5. Open `index.html` with a text editor, find the `SETTINGS` line toward the end, and paste the URL inside `publicCsvUrl: ''`. You can optionally add the regular Google Sheet link to `editorSheetUrl: ''`; note that link will be visible to visitors, although Google still restricts editing by permission.
6. Upload `index.html` to a static web host such as GitHub Pages, Netlify or Cloudflare Pages. For GitHub Pages, place it in a public repository, then enable **Settings > Pages > Deploy from a branch** with main and `/ (root)`.
7. Share the hosted site URL. Visitors need no account to browse or filter annotations. Editors sign into the separately shared Sheet.

Google's published spreadsheet data is public, even if only a small group has editing privileges. Do not publish private research notes, sensitive personal details, or documents you do not have rights to share. PDF links are empty here because the source Word document did not include PDF attachments; add lawful links later in the `file_url` column. Existing URLs found in citations are entered as `article_url` links.

### Behavior and limitations

- Without a Google Sheet connection, the website displays the 71-entry imported snapshot; users can search, filter multiple tags, switch All/Any, filter by publication section, and expand original annotations.
- With a published CSV URL, the website fetches the spreadsheet on page load. If the connection fails, it states that it is showing the imported snapshot, not live data.
- Updates to the published Sheet may take several minutes to propagate. Visitors may need to refresh their browser.
- Edits happen in Google Sheets, not inside the public website. This avoids building custom accounts and an editing backend.
- Full citations have not been independently fact-checked. Do a citation review before publishing publicly.
