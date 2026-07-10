# Morus Paper Privacy Policy

Last updated: July 8, 2026

Morus Paper ("the app", listed on the App Store as Magic Spellbook AI / 魔法书AI笔记) is a handwriting AI notebook app. It lets users write by hand, recognize handwriting, receive AI answers, keep local diary-style notes, and optionally use voice input or call mode.

## Data Stored on Device

The app stores app settings, diaries, recent conversation turns, identity memory, long-term memory cards, and purchase unlock status on the user's device. API keys entered by the user are stored in the iOS Keychain rather than embedded in the app or saved with ordinary preferences. This data is used to provide the notebook, diary, memory, and Pro features.

## Data Sent to Service Providers

By default, handwriting recognition uses iOS on-device OCR. If the user switches to API OCR or a custom OCR provider, the app may send an image of the handwritten page to the configured OCR service.

By default, AI answers use Apple's on-device Foundation Models framework when available. If Apple on-device AI is unavailable, the app may fall back to a local Llama 3.2 3B Instruct Q4_K_M model bundled with the app. Local Llama inference runs on device and does not send prompts to a model download source.

If the user switches to a high-quality API model, the app may send recognized text, necessary recent conversation context, summary memory, and the system prompt to the configured language model service.

When voice input or call mode is used, speech may be processed by Apple's iOS Speech framework, and custom voice model services may receive text that needs to be spoken aloud.

Users may configure compatible third-party model services, such as Alibaba Bailian, for higher-quality OCR, answers, or voice output. Those providers process requests according to their own terms and privacy policies.

## What the App Does Not Do

The app does not include advertising SDKs, does not track users across apps or websites, does not sell personal data, and does not require user account registration.

The developer does not operate a separate server to store user diary content or conversation content. Requests sent to model providers are handled by those providers.

## User Controls

Users can edit, export, or delete diaries in the app. Users can clear memory, restart the first-meeting flow, and revoke microphone or speech recognition permissions in iOS Settings.

Deleting on-device data does not delete request logs that third-party service providers may already have processed.

## Children

The app is not designed specifically for children. Users should not enter sensitive personal information that should not be submitted to third-party model providers.

## Contact

For support or privacy questions, [open a support request](https://github.com/klsk007/mulberry-app-pages/issues/new). Please do not include API keys, private diary text, or other sensitive information.
