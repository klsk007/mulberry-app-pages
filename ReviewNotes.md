# App Review Notes

No account, login, or demo credentials are required.

## App Purpose

Magic Spellbook AI is an iPad handwriting notebook. It lets a user ask a question with Apple Pencil or a finger, watch the original ink fade, and read an AI answer written back on the same page. Conversations can be kept as local daily diary entries. The product-page App Preview demonstrates the core write, fade, and answer flow.

## Main Flow

1. Launch the app. On first launch, tap or write once to wake the page and complete the short naming flow.
2. Write a short question with Apple Pencil or a finger.
3. Stop writing for five seconds to submit automatically, or tap the moon control on the left edge.
4. The handwritten question fades and the answer appears on the same page.
5. Tap the sun control on the left edge to clear the current answer and write again.

The default OCR is Apple's on-device Vision framework. The default answer engine uses Apple's on-device Foundation Models framework when supported. Reviewers can explicitly select Offline Llama in Settings on a physical iPad with at least 5 GiB memory; its approximately 1.9 GB model is then downloaded as an App Store on-demand resource. Users may instead enter compatible API credentials for higher-quality answers or OCR. API credentials are stored in the iOS Keychain.

## Settings And Pro

Tap the star control on the left edge to open Settings. The settings sheet includes page style, language, OCR/model choices, optional Offline Llama download/release controls, diary, memory, About, Privacy Policy, and Terms of Use.

Morus Paper Pro is a one-time, non-consumable lifetime purchase. Open the Pro screen from Settings or by selecting a gated feature. It unlocks call mode, custom OCR, long-term memory and automatic compression, formulas and emoji, and permanent access to all paper styles. The purchase screen includes Restore Purchases.

Black Paper and Morus Paper can be tried for three days before Pro is required. The core handwriting, on-device OCR, and answer flow remain usable without purchase.

## External Services And Frameworks

- Apple Vision provides the default on-device handwriting OCR.
- Apple Foundation Models provides the default answer engine on supported devices.
- Apple Speech and AVFoundation provide optional speech recognition and audio playback.
- StoreKit 2 provides the one-time Pro in-app purchase and Restore Purchases.
- The optional Offline Llama model uses the LlamaSwift/llama.cpp runtime and is delivered by the App Store as an on-demand resource.
- If a user explicitly configures a compatible third-party OCR, language-model, or voice API, the selected provider processes the content needed for that request.

The app has no developer-operated AI backend, account service, advertising SDK, or analytics SDK.

## Regional Availability

Version 1.0 is intended for the United States, Canada, United Kingdom, Australia, New Zealand, Singapore, Taiwan, and Hong Kong. Core app behavior is the same in each storefront. Availability of Apple's on-device language model depends on the review device, OS, and supported language; Offline Llama and user-configured API modes are explicit alternatives.

## Permissions And Data

Microphone and speech-recognition permissions are requested only when the user starts voice input or Pro call mode. No account is required. Diaries, recent conversations, and memory remain on device. The developer does not operate a backend that stores diary or conversation content.

AI output can be inaccurate and is not presented as medical, legal, financial, or other professional advice.

The app is not a regulated healthcare, financial, gambling, insurance, or legal service, so no regulated-industry credentials are applicable.
