📊 Web Excel — Editable, Sortable, Themed Table

A lightweight, browser-based spreadsheet tool built with HTML, JavaScript, jQuery, and DataTables.
This app allows you to load, edit, sort, filter, select, and export tabular data directly in your browser—no backend required.

🚀 Features
📂 File Handling
Import any text-based file (.csv, .tsv, .txt, etc.)
Intelligent parsing of:
Dates
Amounts (supports $, commas, parentheses for negatives)
Automatically detects headers when available
✏️ Editing
Fully editable cells
Inline editing for:
Date
Description
Category
Amount
Action
Automatic formatting:
Dates → YYYY-MM-DD
Currency → $1,234.56
📊 Table Capabilities
Sorting (via DataTables)
Pagination
Search/filter
Dynamic row numbering
Column-based formatting
🎨 Theming
Light / Dark mode toggle
Theme persisted in localStorage
🏷️ Category Highlighting

Auto-coloring for categories like:

Groceries
Gas
Shopping
Food & Drink
Bills & Utilities
Travel
Health & Wellness
And more…
✅ Row Selection System
Select/Deselect rows via checkbox or row click
Bulk actions:
Select All
Deselect All
Select 50% (random or first)
Select N rows
Shift-click range selection
Real-time selected total calculation
➕ Table Editing
Add/Delete rows
Add/Delete columns
Clear entire table
📈 Calculations

Live totals:

💰 Total Amount
📈 Positive Sum
📉 Negative Sum
✅ Selected Rows Total
🔢 Row Count
📤 Export Options
Export to:
CSV
PDF (via html2pdf)
DOC (Word-compatible HTML)
💾 Recent Files System
Stores last 10 files in localStorage
Features:
Auto-load most recent file on startup
View recent files modal
Delete individual entries
Export/import recent files as JSON
⌨️ Keyboard Shortcuts
Shortcut	Action
Ctrl/Cmd + A	Select all rows
Ctrl/Cmd + C	Deselect all
Ctrl/Cmd + H	Select 50%
Ctrl/Cmd + N	Focus "Select N" input
Ctrl/Cmd + E	Export CSV
Ctrl/Cmd + T	Toggle theme

Keybindings can be customized in the KEYBINDS object in the script.

🧠 Internal API

Exposed globally via window.webSheet:

webSheet.loadRows(rows)
webSheet.getRows()
webSheet.selectAll()
webSheet.deselectAll()
webSheet.selectHalf(deterministic)
webSheet.selectN(n)
🛠️ Dependencies

Loaded via CDN:

jQuery
DataTables

Optional (required for PDF export):

html2pdf.js
📦 Installation

No build step required.

Save the file as:

index.html
Open in any modern browser.
⚠️ Notes
PDF export requires html2pdf to be included manually.
Large datasets may impact performance due to DOM rendering.
Data is stored locally (no backend).
🔮 Future Improvements (Ideas)
Column type detection (auto schema)
Drag-and-drop column reordering
Undo/Redo system
Cloud sync support
Chart/graph integration
📄 License

Free to use and modify.

🙌 Disclaimer

 Use at your own risk. Always review scripts before running.
