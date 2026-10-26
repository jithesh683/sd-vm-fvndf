# PFMEA AutoFill Responsive Website

A responsive browser-based helper for PFMEA worksheets.

## Use
1. Open `index.html` in Chrome or Microsoft Edge, or publish the files with GitHub Pages.
2. Import your existing Excel workbook (`.xlsx`, `.xls`, or `.csv`).
3. The tool detects `Product Characteristic`, `Process Characteristic`, `Criteria`, and `Symbol` columns.
4. It suggests `Potential Effects of Failure`, `Severity`, `Revised Detection`, and `Revised Occurrence`.
5. Export a completed copy named `PFMEA_Completed_Same_Format.xlsx`.

## Same-format behavior
The tool writes generated values into matching output columns in the imported workbook and retains other existing worksheet data/sheets where supported. If an output column is missing, it adds that column to the right of the existing header row. Complex Excel formatting, macros, merged cells, and advanced workbook features may not be fully preserved by the browser XLSX library; always check the exported copy.

## Important
- Unrecognized characteristics return `N/A` rather than a generic guess.
- Ratings are preliminary suggestions only. Confirm Severity using your approved customer/company severity table. Revised Detection and Revised Occurrence must reflect actual implemented controls and historical defect data, not assumptions.
- Requires an internet connection to load the SheetJS Excel library from its CDN.
