# Pops & Granny's Thrift Store PWA starter

This is the actual PWA frontend starter staged in this repository.

## Run locally
Serve this directory over HTTP(S) or localhost, for example:
```bash
python3 -m http.server 8080
```
Open `http://localhost:8080`. On supported Android browsers, use Install app / Add to Home screen.

## Included
- Store catalog and item search.
- Local inventory add/remove.
- Checkout basket and local sales log.
- Large-text setting and browser-native speech synthesis.
- Web app manifest, SVG icon, and service worker cache.

## Limitations
This is a frontend starter only. It has no payment processor, tax rules, refunds, authentication, shared database, multi-device synchronization, or reviewed production backend. Browser speech synthesis is a temporary accessibility adapter; the AGAPE engine is not integrated. Demo inventory is sample data. Local records are stored in browser localStorage.

The service worker is an app-shell cache, not a full offline transaction synchronization system. Do not use it as a live POS until persistence, backup/export, audit logging, authentication, data synchronization, and payment workflows are implemented and tested.
