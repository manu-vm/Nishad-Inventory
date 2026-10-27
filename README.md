# Menswear Billing & Stock — Complete ZIP

## Files
- `index.html` — complete responsive billing and stock app, including UPI QR generation.
- `manifest.webmanifest` — installable web app metadata.
- `service-worker.js` — caches the app shell for offline access after the first successful load.

## Deploy on Vercel from GitHub
1. Extract this ZIP.
2. Upload/commit all three files to the **root** of your GitHub repository.
3. Make sure the homepage filename is exactly `index.html` (not `indexx.html`).
4. In Vercel, ensure the project is connected to that repository and the Root Directory is `./` (repository root). For a plain static HTML project, leave the Framework Preset as Other and do not set a custom output directory unless you intentionally deploy from one.
5. Commit changes and wait for the deployment to finish.
6. Open the Vercel URL and refresh.

## UPI QR
Open Settings, enter your UPI ID and payee name, then save. Create a bill and choose **Show UPI payment QR**. The QR library is loaded from cdnjs, so internet is required for QR generation unless the library is bundled locally. Always verify the payment in your bank/UPI app; displaying or scanning a QR does not confirm that money was received.

## Data and backup
Products and bills are stored in the browser on that device, not synced to the cloud. Use Settings → Download data backup (JSON) regularly. Clearing site data may erase records.

## Important
This is a basic billing tool, not certified GST filing/invoicing software. Confirm tax rates and invoice requirements before issuing official tax invoices.
