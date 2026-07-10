# App Store Connect Checklist

## App Information

- Simplified Chinese App Name: 魔法书AI笔记
- Simplified Chinese Subtitle: 会手写回答的咒语笔记
- Simplified Chinese Keywords: 巫师,日记,问答,作业,公式,灵感,占卜,羊皮纸,课堂,学习,OCR,解题,数学,物理
- English App Name: Magic Spellbook AI
- English Subtitle: Handwritten Answers
- English Keywords: wizard,notebook,handwriting,ask,study,homework,formula,diary,journal,paper,chat,question,math,ocr
- In-app brand / skin name: 桑皮纸 / Morus Paper
- Bundle ID: `com.chenbaoliang.mulberry`
- Primary Category: Productivity
- Secondary Category: Education
- Privacy Policy URL: `https://klsk007.github.io/mulberry-app-pages/PrivacyPolicy.html`
- Support URL: `https://klsk007.github.io/mulberry-app-pages/Support.html`
- Terms URL: `https://klsk007.github.io/mulberry-app-pages/TermsOfUse.html`
- License Agreement: Apple Standard EULA is acceptable unless you want a custom EULA.

## In-App Purchase

Create a non-consumable in-app purchase:

- Product ID: `com.chenbaoliang.mulberry.pro.lifetime`
- Reference name: Morus Paper Pro Lifetime
- Display names: Morus Paper Pro / 桑皮纸 Pro / 桑皮紙 Pro
- Type: Non-Consumable
- English Description: Lifetime Pro tools, memory, calls, and skins.
- Simplified Chinese Description: 永久解锁通话、记忆、自定义OCR和全部皮肤。
- Traditional Chinese Description: 永久解鎖通話、記憶、自訂OCR和全部皮膚。
- Base Price: USD 4.99
- Base Territory: United States

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
- Mention external services/frameworks: StoreKit, Apple Speech, AVFoundation, Vision OCR, Apple Foundation Models, the llama.cpp/LlamaSwift runtime, the optional App Store-hosted Offline Llama on-demand asset, and user-configured compatible model APIs.

## Pricing and Availability

- App price: Free.
- Initial availability: United States, Canada, United Kingdom, Australia, New Zealand, Singapore, Taiwan, and Hong Kong.
- Exclude China mainland and the European Union for version 1.0.
- If distributing in China mainland, avoid metadata references to unlicensed foreign AI brands and confirm that model-service availability/compliance is acceptable.

## Export Compliance

The app uses standard Apple networking/TLS and does not implement custom encryption. `ITSAppUsesNonExemptEncryption` is set to `false` in `Info.plist`.
