# Register Scanner

A mobile-first progressive web app for capturing a register page, running English OCR, reviewing/correcting the extracted text, and exporting CSV for Google Sheets.

## Features
- Mobile camera capture or image upload
- Image contrast enhancement before OCR
- Editable OCR output for manual correction
- CSV export with one non-empty scanned line per row
- PWA manifest and service worker for adding the app to an Android home screen

## Run
Open the deployed HTTPS site on Android Chrome. Choose a register photo, tap **Scan photo**, review and correct the text, then download the CSV.

OCR uses Tesseract.js from a CDN, so an internet connection is needed to load the OCR library and language data. This version is optimized for printed English; handwriting and Urdu may be inaccurate. Always compare extracted names and numbers with the original register.

## Enable GitHub Pages
In the repository settings, open **Pages**, select **Deploy from a branch**, choose **main** and **/(root)**, then save. After GitHub publishes the site, open the Pages URL on Android Chrome and choose **Install app** or **Add to Home screen** from the browser menu.

CSV is an intermediate file; it is not sent directly to Google Sheets. Import/open the downloaded CSV in Google Sheets.
