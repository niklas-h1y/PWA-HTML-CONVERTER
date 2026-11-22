# Base URL Converter

A minimalist, browser-based PWA that updates the **first** `<base>` element in an uploaded HTML file.

## Use

1. Enter a destination URL (http:// or https://).
2. Choose or drop an `.html` / `.htm` file.
3. Select **Convert & download**.

The converter changes only the first `<base>` tag. If that tag has an `href` attribute, its value is replaced. If it has no `href`, one is added. If no `<base>` tag exists, the converter reports that and leaves the file unchanged.

All file processing happens locally in your browser; no file is uploaded to a server.

## PWA

The app includes a web app manifest and a service worker for installability and offline app-shell caching. Serve it over HTTPS (or localhost) to enable PWA features.
