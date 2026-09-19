# LoveMatch
Open `index.html` directly for the offline app. All code and images are local. No server, API, CDN, database, payment gateway, Xendit, GCash or webhook is included. The scoring engine is separated from result rendering so a future payment gate can be inserted before the result screen.


## Optional GCash Donation Screen
The result flow now includes an optional donation screen before the result. Users can skip it and see the result immediately. To use your own GCash QR code, replace `assets/gcash-qr.svg` with your QR image and keep the same filename (or update the `<img>` source in `index.html`). No payment verification, backend, API, or database is required for this donation-only version. GitHub Pages can host the site as a static website.


## GCash donation screen
- Uses the supplied GCash/Instapay QR image in `assets/gcash-qr.jpg`.
- Displays GCash number `09380536208` with a copy button.
- Donation is optional: **Skip** opens the result immediately.
- **Yes, I'd like to support** reveals the QR and number, then the user can continue to the result.
- This is a static donation flow; it does not verify payment or require a backend.
