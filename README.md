# Testing Prep Toolkit V9

A static HTML/CSS/JavaScript toolkit for GitHub Pages. V9 expands the Engineering File Generator with document-count, page-count, discipline and tagging controls.

## What's included

- **Engineering File Generator:** select multiple formats, choose how many separate documents to generate and how many pages each document should contain, assign a discipline and comma-separated tags, generate blank or populated starter documents, preview filenames, and download individually or as a ZIP. Supports PDF, DOC/DOCX, XLS/XLSX, CSV, TXT, HTML, JSON, XML, JPG, PNG, TIF/TIFF and DXF; DWG can be copied from a user-supplied template.
- Package name generator using `CS_USxxxxx_TCxx_ddmmyy_hhmmss`, with current local timestamp or manual date/time.
- DataURL Studio: image preview, rotate, flip, crop (freeform and preset ratios), resize, encoding, output optimisation, batch conversion and Data URL inspection.
- Beginner testing Learning Pathway.
- Searchable Testing Reference Guide.
- **My Notes page:**
  - Create multiple notes; rename and delete them.
  - Organise notes into folders/categories such as Learning, Work Notes, Meetings, Testing Tasks, Technical Reference and To Remember.
  - Add your own folders.
  - Rich-text editor with bold, italic, underline, headings, font size, text colour, highlighting, bullets, numbered lists, checklists, tables, code blocks, hyperlinks, undo and redo.
  - Autosave to the current browser, with HTML export for individual notes.
- **Testing Process page:**
  - Editable standard end-to-end testing workflow covering requirements, planning, test design, environment/data preparation, execution, defect reporting, retesting, regression and closure/reporting.
  - Separate **Our Team Process** area where you can add, rename, edit, reorder and delete stages.
  - Rich-text formatting in both standard and team process stages.
  - Practical starting templates for test cases, defect reports, smoke testing, regression planning, UAT preparation and pre-testing readiness. Templates can be added as editable stages to your team process.
  - Autosave plus explicit save controls and HTML export of the team process.
- Test execution checklist.
- Complete JSON backup and restore for notes, folders, process pages and checklist state. Older V6 backups with the previous single notes field are also accepted.

## Run locally

Open `index.html` in a modern browser. Clipboard functionality works best on HTTPS or localhost.

## Publish on GitHub Pages

1. Upload `index.html` and this README to the repository.
2. In repository Settings → Pages, choose Deploy from a branch, select `main` and `/ (root)`, then save.

## Data, privacy and compatibility

- Image processing happens locally in the browser; images are not uploaded.
- Notes and process content are saved in browser local storage on the current device/browser. GitHub Pages does not sync data between devices.
- Use **Data & backup** to export/import a JSON backup before changing browsers or devices.
- Do not store passwords, secrets or real customer/personal data in this tool.
- Browser canvas output supports PNG, JPEG and WebP in modern browsers. Animated GIFs may be flattened; TIFF/ICO/BMP support depends on browser decoding.

## Editing guidance

The standard workflow is intended as a generic starting point, not a replacement for your organisation's process. Edit it to suit your needs, and document the team's actual workflow separately under **Our Team Process**. Always follow your organisation's policies, agreed entry/exit criteria, defect definitions and data-handling rules.


## Engineering file generator notes

- DOC and XLS are HTML-based compatibility files, not legacy binary Office files. DOCX and XLSX are genuine Office Open XML packages.
- PDF, DOC, DOCX and HTML populated documents support the selected page count; DOC/DOCX and PDF include page breaks. The selected discipline and tags are included in populated document content (and as structured fields in JSON). Blank mode creates blank documents with the requested page count where the format supports pages.
- DWG is not generated from scratch: upload a valid DWG template to create a renamed copy. DXF is generated directly.
- ZIP and DOCX/XLSX packaging uses JSZip loaded from jsDelivr; an internet connection is required for those packaging features. Other simple file types can be generated without it.
- Blank raster image files are valid blank images; the TIFF output is a minimal 1×1 TIFF.
