# Mouklis Browser — Legal Notices & Open-Source Compliance

**Version 1.0 | Android 13+ | x86_64 / ARM64**

Mouklis Browser is a desktop-style web browser developed for **Mouklis OS**, powered by the Cefrium SDK and Chromium.

This repository provides third-party license notices, copyright attributions, upstream source references, and binary relinking materials for Mouklis Browser 1.0.

**This is not the Mouklis Browser application source-code repository.** The original proprietary application source code is not published here.

## 1. Browser Engine & Third-Party Components

Mouklis Browser uses the following components:

- **Cefrium SDK 0.19.0** — Licensed under LGPL-3.0-or-later.
  - [Cefrium Official Website](https://cefrium.com)
  - [Cefrium Source Code](https://codeberg.org/cefrium/cef-android)
  - [Cefrium v0.19.0 Source](https://codeberg.org/cefrium/cef-android/src/tag/v0.19.0)

- **Chromium 156.0.8078.80** — Distributed through Cefrium under BSD-style and other applicable third-party licenses.
  - Full copyright notices and license information are available in `CHROMIUM_THIRD_PARTY_CREDITS.txt`.

- **AndroidX, Google Play services, Firebase, ML Kit, and other dependencies** — Used under their respective licenses and applicable terms.

For detailed component attribution, see `THIRD_PARTY_NOTICES.md`.

Complete applicable license texts are provided in the `LICENSES/` directory.

## 2. LGPL Compliance & Relinking Materials

Cefrium SDK is used under the terms of the GNU Lesser General Public License, version 3 or later (LGPL-3.0-or-later).

To support the applicable LGPL relinking requirements, this repository provides a Binary Relinking Kit containing:

- Compiled Mouklis Browser application classes.
- Required application resources and build configuration.
- Gradle build instructions.
- Configuration for building against a compatible modified Cefrium SDK.

**Binary Relinking Kit:**

[View Relinking Materials](relink-kit/)

The compiled application materials are provided for relinking purposes, including reverse engineering necessary to debug modifications to LGPL-covered components, as permitted by the applicable license.

The original Mouklis Browser Java/Kotlin source code is not included.

For further information about LGPL obligations and source availability, see `SOURCE_AND_LGPL_INFORMATION.md`.

## 3. Proprietary Application Code

Mouklis Browser is independently developed as part of the Mouklis OS project.

Its original application source code, proprietary interface components, and independently developed features remain closed source.

The publication of third-party license notices and binary relinking materials does not place the entire Mouklis Browser application under an open-source license.

Third-party components continue to be governed by their respective licenses. Rights necessary to comply with LGPL are preserved.

## 4. Trademarks & Intellectual Property

The names **Mouklis**, **Mouklis Browser**, **Mouklis OS**, and their associated logos and visual identities belong to the Mouklis project owner.

No trademark license is granted through this repository.

Third-party names, trademarks, and copyrighted materials remain the property of their respective owners.

See `TRADEMARKS.md` for additional information.

## 5. Distribution & License Information

Mouklis Browser is intended to be included as a browser within Mouklis OS.

The repository provides legal notices, third-party license information, source references, and application relinking materials associated with version 1.0.

The independent build using the original Cefrium SDK 0.19.0 was successfully completed. The provided relinking materials include instructions for building against a compatible modified Cefrium SDK.

Distribution remains subject to the applicable third-party licenses, including LGPL requirements concerning corresponding source and relinking.

For more information, refer to:

- `THIRD_PARTY_NOTICES.md`
- `SOURCE_AND_LGPL_INFORMATION.md`
- `CHROMIUM_THIRD_PARTY_CREDITS.txt`
- `LICENSES/`
- `relink-kit/`
- `TRADEMARKS.md`

---

**Mouklis Browser © 2026 Mouklis Project.**

Third-party software and libraries retain their respective copyright notices and license terms.
