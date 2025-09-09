Step 4: Metadata Extraction

Tools used: metagoofil, exiftool

Used Google Dorks and Metagoofil to search for documents (pdf,docx,pptx).

Downloaded files into metagoofil_output/.

Extracted metadata using:

exiftool *.pdf > metadata_report.txt

Findings:

Author/usernames from documents

PDF producer software

Creation/modification timestamps

(If no files found → “No publicly available documents with metadata were identified.”)
