# App Review Notes

No account, login, or demo credentials are required.

## Main Flow

1. Launch the app. On first launch, tap or write once to wake the page and complete the short naming flow.
2. Write a short question with Apple Pencil or a finger.
3. Stop writing for five seconds to submit automatically, or tap the moon control on the left edge.
4. The handwritten question fades and the answer appears on the same page.
5. Tap the sun control on the left edge to clear the current answer and write again.

The default OCR is Apple's on-device Vision framework. The default answer engine uses Apple's on-device Foundation Models framework when supported. When Apple on-device AI is unavailable, the app can use its bundled Llama 3.2 3B Instruct Q4_K_M model on devices with sufficient memory. Users may optionally enter their own compatible API credentials in Settings for higher-quality answers or OCR. API credentials are stored in the iOS Keychain.

## Settings And Pro

Tap the star control on the left edge to open Settings. The settings sheet includes page style, language, OCR/model choices, diary, memory, About, Privacy Policy, and Terms of Use.

Morus Paper Pro is a one-time, non-consumable lifetime purchase. Open the Pro screen from Settings or by selecting a gated feature. It unlocks call mode, custom OCR, long-term memory and automatic compression, formulas and emoji, and permanent access to all paper styles. The purchase screen includes Restore Purchases.

Black Paper and Morus Paper can be tried for three days before Pro is required. The core handwriting, on-device OCR, and answer flow remain usable without purchase.

## Permissions And Data

Microphone and speech-recognition permissions are requested only when the user starts voice input or Pro call mode. No account is required. Diaries, recent conversations, and memory remain on device. The developer does not operate a backend that stores diary or conversation content.

AI output can be inaccurate and is not presented as medical, legal, financial, or other professional advice.
