# App Privacy Answers

Use these answers for the current 1.0 binary. Recheck them if analytics, a developer server, accounts, or a bundled cloud API key is added later.

## Data Collection

Answer **Yes, data is collected** because optional user-configured OCR, language-model, and voice providers can receive content from the app. The developer does not operate an analytics or advertising backend and does not sell data.

## Declare This Data Type

- **User Content -> Other User Content**
- Examples: handwriting page images, recognized text, prompts, necessary conversation context, memory summaries, and text sent to a custom voice provider.
- Purpose: **App Functionality** only.
- Linked to the user: **Yes** as the conservative answer. A user-supplied provider API key can associate requests with that provider account even though Morus Paper has no account system.
- Used for tracking: **No**.

## Do Not Declare For This Binary

- **Audio Data:** microphone audio is used for real-time Apple Speech recognition and is not retained or sent to the developer's server. Custom voice providers receive answer text, not microphone audio.
- **Purchase History:** StoreKit verifies the Pro entitlement on device; the developer does not receive or store purchase history on a separate server.
- **Identifiers, diagnostics, usage data, location, contacts, financial information, health, browsing history, or search history:** the app does not collect these data types.

## Tracking

Answer **No**. The app has no advertising SDK, analytics SDK, ATT request, data broker integration, or cross-app tracking.

## Notes

- Local diaries, recent conversations, memory cards, settings, and API credentials stay on device. API credentials are stored in Keychain.
- On-device Vision OCR, Apple Foundation Models, and the optional App Store-hosted Offline Llama asset do not send prompts to the developer or to the model download source.
- The privacy policy explains when optional third-party services receive user content.

## Privacy Manifest In App Bundle

The app includes `PrivacyInfo.xcprivacy` with:

- `NSPrivacyTracking = false`
- `NSPrivacyAccessedAPICategoryUserDefaults` reason `CA92.1`
