# App Review Notes Draft

No account is required.

## 1. Physical Device Screen Recording

Please attach a short physical-device recording that starts from launching the app and shows:

1. First launch / onboarding prompt.
2. Writing a question by hand on the page.
3. Tapping the moon/read button and seeing ink fade.
4. AI answer appearing on the same page.
5. Opening Settings from the left-side button.
6. Opening About, Privacy Policy, and Terms of Use.
7. Opening the Pro purchase screen and using Restore Purchases.
8. Optional: voice input permission prompt and call mode.

## 2. App Purpose

Magic Spellbook AI / 魔法书AI笔记 is an iPad handwriting AI notebook internally branded as Morus Paper / 桑皮纸. It provides a minimal paper-like interface where users write questions by hand, the app recognizes the handwriting, and the answer is written back onto the page. By default it uses iOS on-device OCR and Apple's on-device Foundation Models framework. If Apple on-device AI is unavailable, it can fall back to a local Llama 3.2 3B Instruct Q4_K_M model bundled with the app and running on device. Users can optionally configure compatible API services for higher-quality OCR or language model answers. It also saves daily diary-style notes and local memory so repeated conversations feel continuous.

## 3. Access Instructions

No login or demo account is required.

To test the main feature:

1. Launch the app.
2. If onboarding appears, answer the first prompt or skip the guide.
3. Write a short question on the page.
4. Tap the moon/read button on the left side.
5. Wait for the handwritten answer to appear.

To test Settings:

1. Tap the settings button on the left side.
2. Change page color, language, writing settings, and recognition language.
3. Open About to view privacy and terms.

To test Pro:

1. Open Settings.
2. Tap the Pro unlock entry or any gated Pro feature, such as Call Mode or Custom OCR.
3. The purchase screen explains the lifetime Pro unlock and includes Restore Purchases, Privacy Policy, and Terms of Use.

## 4. External Services

The app uses Apple StoreKit for in-app purchase, Apple's Speech framework for speech recognition permission and transcription, Apple's AVFoundation for microphone and text-to-speech/audio playback, Apple's Vision framework for default on-device OCR, Apple's Foundation Models framework for default on-device answers, and llama.cpp/LlamaSwift for the local Llama fallback model. Users may optionally configure compatible API services such as Alibaba Bailian for higher-quality model answers, OCR, or custom voice output.

The app does not require account registration and does not operate a developer-hosted backend server for diary or conversation storage. API keys entered by the reviewer are stored in the iOS Keychain and are not embedded in the app binary.

## 5. Regional Differences

The app's default Apple on-device experience depends on iOS/Apple Intelligence availability on the user's device. The local Llama fallback is bundled with the app and is enabled only when the device has enough physical memory; lower-memory devices can use a user-configured API instead. Optional API model availability may depend on the user's network, region, and third-party provider configured in Settings.

## 6. Regulated Industry

The app is not a medical, legal, financial, gambling, insurance, or regulated professional service. AI answers are for learning, writing, and everyday companionship only and should not be treated as professional advice.
