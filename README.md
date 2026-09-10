# GoldPulse AI — iPhone PWA Live Test

This is a phone-friendly Progressive Web App.

## Current test features
- Live indicative XAU/USD price from `https://api.gold-api.com/price/XAU`
- 30-second refresh
- BUY / SELL / WAIT estimate
- BUY LIMIT / SELL LIMIT / BUY STOP / SELL STOP generator
- Entry, SL, TP1, TP2, TP3
- M1, M5, M15, M30, H1, H4, D1, W1 estimated bias
- Local history stored on the iPhone
- WebAuthn platform biometric setup (Safari can use Face ID on supported iPhones)
- Home Screen/PWA support

## Important limitation of this test
The free endpoint provides live price/daily market fields, but this test build does not download full broker-grade candle history for every timeframe.
Short-term timeframe estimates improve as the app stays in use because it stores live observations locally.
Do NOT treat these generated levels as guaranteed or broker-executable prices.

## To use as an iPhone Home Screen app
The files must be hosted on HTTPS. WebAuthn/Face ID also requires a secure origin.

Upload the contents of this folder to any HTTPS static host. Then:
1. Open the HTTPS site in Safari on iPhone.
2. Tap Share.
3. Tap Add to Home Screen.
4. Open GoldPulse AI from the Home Screen.
5. Tap Enable / Unlock with Face ID.
6. Approve Face ID.

## Data source
Gold API: https://gold-api.com/
Prices are indicative. Use XM/MT5 demo account prices when comparing signal levels.
