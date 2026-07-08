# App Store Connect Checklist

## App Information

- App name: 桑皮纸 / Mulberry
- Bundle ID: `com.chenbaoliang.mulberry`
- Category suggestion: Productivity or Lifestyle
- Privacy Policy URL: `https://klsk007.github.io/mulberry-app-pages/PrivacyPolicy.html`
- Support URL: `https://klsk007.github.io/mulberry-app-pages/Support.html`
- Terms URL: `https://klsk007.github.io/mulberry-app-pages/TermsOfUse.html`
- License Agreement: Apple Standard EULA is acceptable unless you want a custom EULA.

## In-App Purchase

Create a non-consumable in-app purchase:

- Product ID: `com.chenbaoliang.mulberry.pro.lifetime`
- Reference name: Mulberry Pro Lifetime
- Display name: Mulberry Pro
- Type: Non-Consumable
- Description: Lifetime unlock for call mode, custom OCR, long-term memory, automatic memory compression, formula and emoji output, and permanent Black Paper and Mulberry Paper skins.

Make sure the IAP is attached to the app version before review.

## Product Page

Required:

- iPad screenshots showing actual use, not only concept art.
- Description should mention handwriting AI notebook, diary, memory, voice/call mode, and Pro unlock.
- Avoid AI brand names in metadata if distributing in China mainland.
- Support URL: `https://klsk007.github.io/mulberry-app-pages/Support.html`

## Review Information

- No demo account is required.
- Add the text from `AppStore/ReviewNotes.md`.
- Attach a real-device screen recording link.
- Mention external services: StoreKit, Apple Speech, AVFoundation, Alibaba Bailian, optional user-configured compatible model APIs.

## Pricing and Availability

- App price: choose free if using Pro IAP.
- If distributing in China mainland, avoid metadata references to unlicensed foreign AI brands and confirm that model-service availability/compliance is acceptable.

## Export Compliance

The app uses standard Apple networking/TLS and does not implement custom encryption. Answer export compliance accordingly in App Store Connect.
