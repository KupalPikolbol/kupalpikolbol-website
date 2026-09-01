# Kupal Pikolbol Website — GitHub Frontend

This `index.html` is a standalone copy of the current working customer website.

## Important safety rule

The existing Google Apps Script booking backend is **not replaced or deleted**.

The frontend has an API bridge so the existing `google.script.run(...)` calls can later be routed through HTTP without rewriting the whole customer UI.

## Current status

- Design/UI: copied from the current working customer page.
- Booking UI: preserved.
- GCash UI/QR modal: preserved.
- Calendar/court/time selection: preserved.
- Check My Booking: preserved.
- Existing Apps Script backend: untouched.
- Shared API secret: intentionally **not included** in this public GitHub file.

## Before production

The current Apps Script API requires a shared key. Do **not** put that key into `index.html`, because this GitHub repository is public.

A secure server-side proxy/API layer must be placed between GitHub Pages and Apps Script before connecting the production domain.

## GitHub upload

Upload:

- `index.html`
- this README if desired

Do not change the live Apps Script deployment while testing the GitHub version.
