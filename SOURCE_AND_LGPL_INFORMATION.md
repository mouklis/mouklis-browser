# Cefrium / LGPL source and distribution information

Version identified in the supplied project and APK: **Cefrium SDK 0.19.0**, embedding Chromium **156.0.8078.80**, x86_64 native `libcef.so`.

- Cefrium upstream project: https://codeberg.org/cefrium/cef-android
- Version-specific source reference: https://codeberg.org/cefrium/cef-android/src/tag/v0.19.0
- Cefrium release history: https://cefrium.com/releases/
- Cefrium licence and trademark policy: https://cefrium.com/policy/
- LGPL-3.0-or-later: `LICENSES/LGPL-3.0-or-later.txt`
- GPL-3.0-or-later (referenced by LGPLv3): `LICENSES/GPL-3.0-or-later.txt`
- Chromium and third-party licences: `CHROMIUM_THIRD_PARTY_CREDITS.txt` and `THIRD_PARTY_NOTICES.md`.

Cefrium's own source and licence are distinct from Mouklis Browser application code. A proprietary application can interact with an LGPL-licensed library subject to the actual terms of LGPLv3, including LGPLv3 section 4 for combined works.

The LGPLv3 section 4 options depend on the linking and redistribution arrangement. In particular, merely placing a third-party source-code URL in a public GitHub repository is **not a substitute** for the corresponding source requirements and a valid relinking or replaceable shared-library arrangement. For an Android APK combining Java/Kotlin code and a packaged native library, the actual SDK packaging, Dex/Java linkage, ability to rebuild or replace the library, required corresponding application object code (if applicable), and any installation information must be assessed against the actual final build.

This repository records source information and notices; **it does not by itself fulfill or certify all distribution obligations**. The exact 0.19.0 source, applicable source distribution method and LGPL section 4 compliance must be checked before distributing the final closed-source APK. If an LGPL-covered component was modified, the corresponding modified source and change notices must also be provided under applicable terms.

Technical metadata: the unsigned pre-release APK inspected in preparation of this notices bundle has SHA-256 `616573e570875c494f03f7ce28dec37c3e67b3e40a94b31cfc8433cabe7272b7`. This fingerprint identifies the inspected pre-release artifact only, not a future corrected/signed release.
