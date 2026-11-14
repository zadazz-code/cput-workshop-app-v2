# CPUT Workshop App v2

The v2 storeroom app for the Product and Industrial Design workshop. This is a separate app from the live storeroom app, with its own Google Sheet ("Tool Signout V2") and Apps Script backend.

## Files
- `index.html`: the staff app (v2 layout and styling). The backend URL is set in the `const API` line near the top of the script.
- `guide.html`: the staff guide.
- `apps-script/tool-checkout-code-v20.js`: the backend. Paste it into the Apps Script project bound to the "Tool Signout V2" Sheet.
- `manifest.json`, icons and `logo.png`: app icons and branding.

## Setup
1. Make the "Tool Signout V2" Google Sheet and bind an Apps Script project to it.
2. Paste in `apps-script/tool-checkout-code-v20.js`.
3. Deploy > New deployment > Web app. Execute as: Me. Access: Anyone. Copy the `/exec` URL.
4. Replace the placeholder in the `const API` line of `index.html` with that URL, then host the site.

Until step 4 is done, the app cannot reach a backend.
