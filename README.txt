MY FOOD LOG — VS CODE STARTER

Files:
- index.html: the whole starter app (HTML, CSS, JavaScript).

Run it:
1. Extract the ZIP.
2. Open the folder in VS Code.
3. Install the "Live Server" extension (if you don't already have it).
4. Right-click index.html and choose "Open with Live Server".
5. Allow camera access when prompted. Camera access usually works on localhost; a deployed site needs HTTPS.
6. Click Open camera to scan a barcode, or type the barcode and click Find product.
7. Check the returned nutrition against the product package, enter the amount you ate, and click Save to diary.

How it works:
- Uses Open Food Facts' public product API to look up barcode data.
- Uses html5-qrcode from a CDN for camera barcode scanning.
- Stores entries in this browser's localStorage; it is not cloud-synced.
- Exports diary entries as CSV.

Accuracy notes:
- No app can promise 100% food-tracking accuracy. Barcode databases can be incomplete or wrong.
- The app uses nutrition values per 100 g where available, then scales them to the amount entered.
- Missing values show as zero, so always verify the label and fill in any missing nutrition manually.
- This is a starter project, not a medical device or a substitute for professional dietary advice.
- It requires an internet connection for the scanner library and online product lookup.
