# Finance Apps: ARAP, Pool and ACCRUAL

This folder contains everything required for the combined Streamlit app.

## Upload to GitHub

1. Extract the ZIP on your computer.
2. Open the extracted folder. You should see these three files:

   finance_app.py
   requirements.txt
   README.md

3. In your GitHub repository, choose Add file > Upload files.
4. Select all three files and upload them to the repository's main level.
5. Replace the existing files with these versions and commit the changes.

Upload the three files themselves. There are no subfolders to preserve.
You do not need to upload the ZIP, separate app folders, or Excel reference files.
The app code and all required reference workbooks are embedded in finance_app.py.
Old loose files from previous uploads are not needed by this version.

## Streamlit deployment

Set the main file path to:

finance_app.py

Use the repository and branch containing the uploaded files.
If an existing deployment still shows an old error after updating, reboot it.

## Using the app

The top navigation provides Home, ARAP, Pool and ACCRUAL.
Each app also has its own path: /arap, /pool and /accrual.
Open them in separate browser tabs to keep independent uploads and inputs.
Switching apps within one browser tab can reset inputs and uploads.

## Run locally

Use Python 3.10 or newer:

python -m pip install -r requirements.txt
python -m streamlit run finance_app.py

## Included reference files

ARAP and ACCRUAL each contain their own company mapping, account mapping,
AX template and D365 template. Pool contains its own company mapping.
No external reference-file folders are needed for deployment.

## Redcare corporate layout

The shared Home, ARAP, Pool and ACCRUAL pages use the Redcare colour palette:
off-white (#FFEEE8), brown (#2B140E), peach (#FFC7B1), and red (#ED0334) accents.
The official Redcare logo and Redcare Accessible fonts are embedded in
finance_app.py, together with the responsive layout and styling. No additional
files, folders or font-service connections are needed for deployment.

The update includes a branded header, workflow cards, matching upload controls,
result metrics and download buttons, plus a mobile layout.

Brand sources:
- https://redcare.hypedev.23x.me/colour/
- https://redcare.hypedev.23x.me/typography/
- https://redcare.hypedev.23x.me/logo/

## Validation

The standalone app was tested from a folder containing only finance_app.py and
requirements.txt. ARAP, Pool and ACCRUAL each processed a sample workbook and
provided downloads. Navigation and widget reruns were also checked.

The corporate layout was also inspected in a browser at desktop and mobile widths.
