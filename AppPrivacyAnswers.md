# App Privacy Answers Draft

Use this as a conservative starting point for App Store Connect App Privacy.

## Data Collection

The developer does not run an analytics or advertising backend and does not sell or track user data across apps.

However, the app sends user content to third-party model services when the user uses OCR, AI answer, or custom voice features. App Store Connect may consider that data "collected" by third parties. Fill this honestly based on the final provider configuration.

## Likely Data Types

- User Content: handwriting page images, recognized text, prompts, AI conversation context, diary-derived memory summaries when needed for AI responses.
- Audio Data: voice input may be processed through Apple's Speech framework; custom voice/call features may process speech-derived transcripts and speech output text.
- Purchase History: StoreKit purchase status for Pro unlock.

## Usage Purposes

- App Functionality: OCR, AI answers, voice/call mode, Pro unlock restoration, diary and memory features.
- Not used for third-party advertising.
- Not used for tracking across apps and websites.

## Tracking

Answer "No" for tracking if no ad SDK, analytics SDK, ATT usage, or cross-app tracking domain is added.

## Linked to User

If no account system is added, local diaries and memory are not linked to a developer account. Third-party model providers may process requests according to their own policies. If App Store Connect asks whether provider-processed user content is linked to the user, answer according to the final provider's account/API setup.

## Privacy Manifest In App Bundle

The app includes `PrivacyInfo.xcprivacy` with:

- `NSPrivacyTracking = false`
- `NSPrivacyAccessedAPICategoryUserDefaults` reason `CA92.1`
