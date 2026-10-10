# AASE Stream Tracker

This starter site implements two distinct datasets:
- **First Time Cleared**: role (AASE only), stream, on/off campus, Gear Up mail Yes/No.
- **Retest**: role (AASE only), stream, on/off campus, Gear Up mail Yes/No, HON/Caps/VIVA/result dates.
- Blank retest dates are saved as blank. Use the generated retest record ID to fill in dates later.
- Per-stream counts appear directly below each section's form. There is no separate community statistics page.
- First Time Cleared has four counters per stream: on-campus received, off-campus received, on-campus not received, off-campus not received.
- Retest counts split by campus, Gear Up Yes/No, and completed/not completed. “Completed” means the Retest Result date is filled.

## Set up free hosting/storage
1. Create a Google Sheet.
2. In the sheet choose **Extensions → Apps Script**. Replace `Code.gs` with the included code and save.
3. In Apps Script **Project Settings → Script Properties**, add `SPREADSHEET_ID` with the ID from the Sheet URL.
4. Deploy as **Web app**, execute as **Me**, access **Anyone** if your account allows it. Copy the `/exec` URL.
5. In `index.html`, replace `PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE` with that URL.
6. Publish `index.html` through GitHub Pages (upload to a repository, then enable Pages in repository Settings). Share the resulting website link.

## Important
This is a public, user-reported tracker, not an official or verified company system. Public links can be shared beyond the intended groups, and this basic version has no robust anti-spam or duplicate-submission protection. Do not collect names, email addresses, employee IDs, phone numbers, or confidential information. Apps Script/GitHub quotas and access policies may change.
