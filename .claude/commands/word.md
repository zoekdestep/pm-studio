---
description: Export a markdown file to Word and open it
arguments:
  - name: file
    description: The markdown file to export (path or filename)
    required: false
---

Export a markdown document to Word format and open it immediately.

## Process

1. **Identify the file to export:**
   - If `$ARGUMENTS.file` is provided, use that file
   - Otherwise, check if the user has a file open in the IDE and use that
   - The file should be a markdown (.md) file

2. **Convert to Word:**
   - Use pandoc to convert the markdown file to .docx format
   - Save the Word file to `/output/` with the same base name
   - Example: `notes/research/my-doc.md` → `output/my-doc.docx`

3. **Open the file:**
   - Use `open` command to launch the Word document immediately

4. **Confirm:**
   - Tell the user where the file was saved and that it's been opened

## Example

User runs: `/word`
(with `notes/research/2026-01-09-experiment.md` open in IDE)

Result:
- Creates `output/2026-01-09-experiment.docx`
- Opens it in Word
- Confirms: "Exported to output/2026-01-09-experiment.docx and opened in Word."
