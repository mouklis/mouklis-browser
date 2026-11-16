# Third-party notices

Mouklis Browser 1.0 (`com.mouklis.browser.v2`). This repository publishes third-party notices only, not the proprietary browser source code.

The Mouklis Browser application source is not included here. The third-party software listed below retains its respective licences.
Full licence texts are in `LICENSES/`. Component metadata was recorded in a project dependency review dated 2026-11-15 and matched against selected assets in the supplied unsigned release APK. This does not independently establish full compliance for distribution.

The browser provides its licences page under Settings > About Mouklis > Open source licences (`mouklis://licenses`). Before distributing a signed release, verify that its built-in notices match this repository and that all LGPL distribution conditions have been satisfied.

## 1. Cefrium SDK 0.19.0

- Artifacts: `com.cefrium:cefrium-sdk`, `cefrium-sdk-core`, `cefrium-native-codecs-x86_64`, `cefrium-native-codecs-arm64-v8a`, `cefrium-native-codecs-armeabi-v7a` (version 0.19.0). The build-time Gradle plugin `com.cefrium:cefrium-gradle-plugin` 0.19.0 is not packaged.
- Copyright: 2026 Juan Manuel Méndez Rey (from the SDK source headers).
- Licence: **LGPL-3.0-or-later** (package metadata). The source headers read `SPDX-License-Identifier: LGPL-3.0-or-later OR LicenseRef-Cefrium-Commercial`; Mouklis Browser uses the SDK under LGPL-3.0-or-later.
- Licence texts: `LICENSES/LGPL-3.0-or-later.txt` and `LICENSES/GPL-3.0-or-later.txt` (the LGPL builds on the GPL).
- Source code of the SDK: https://codeberg.org/cefrium/cef-android (project site https://cefrium.com).
- The inspected project declares Cefrium SDK 0.19.0 as a Gradle dependency. The developer has not provided evidence of a modified Cefrium SDK. See `SOURCE_AND_LGPL_INFORMATION.md` for upstream source and outstanding LGPL compliance checks.

## 2. Chromium and its bundled components

- Cefrium 0.19.0 embeds **Chromium 156.0.8078.80** (`libcef.so` and the `.pak` resources).
- Chromium's own code ("The Chromium Project") is under a BSD-style licence (`LICENSES/BSD-3-Clause.txt`).
- Chromium bundles 769 third-party components. Their notices and full licence texts are included in `CHROMIUM_THIRD_PARTY_CREDITS.txt`, generated from the credits data packaged within the inspected APK; the in-app licences page also shows them under **Chromium credits**.
- Licence types in those credits include: Apache-2.0, MIT, BSD-2-Clause, BSD-3-Clause, Unicode-3.0 (ICU), curl, ISC, Zlib, CC0-1.0, BSL-1.0, FTL, EPL-1.0, OFL-1.1, MS-PL, libtiff, X11, blessing (sqlite), CC-BY-3.0, CC-BY-4.0, CC-BY-SA-3.0, MPL-1.1, MPL-2.0, LGPL-2.0-or-later, LGPL-2.1-or-later, LGPL-3.0-or-later, GPL-2.0-or-later, GPL-3.0-or-later, plus a few project-specific licences shown in full in the credits (Ooura FFT, Anti-Grain Geometry, HarfBuzz "Old MIT", UnRAR).
- Components under LGPL named in the credits include ffmpeg (LGPL-2.1-or-later), WebKit, liblouis (Braille Translation Library, LGPL-3.0), hunspell dictionaries, Netscape Portable Runtime (NSPR) and symphonia.
- Components under MPL named in the credits include hunspell (MPL-1.1), NSPR, Eigen, symphonia and Mozilla Personal Security Manager.
- EasyList is listed as dual GPL-3.0-or-later / CC-BY-SA-3.0. UnRAR's licence forbids using its code to build a RAR-compatible archiver.

## 3. Google Play services, Firebase, ML Kit and Play Core

These libraries are **not** open source. They are not added by Mouklis Browser: `com.cefrium:cefrium-sdk-core:0.19.0` declares them as runtime dependencies, so they are packaged with it. They are used under Google's terms:

| Artifact | Version | Terms |
|---|---|---|
| `com.google.android.gms:play-services-auth-api-phone` | 18.3.1 | Android Software Development Kit License, https://developer.android.com/studio/terms.html |
| `com.google.android.gms:play-services-auth-base` | 18.3.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-base` | 18.11.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-basement` | 18.12.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-cast` | 22.2.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-cast-framework` | 22.2.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-clearcut` | 17.0.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-cloud-messaging` | 17.4.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-flags` | 18.1.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-gcm` | 17.0.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-identity-credentials` | 16.0.0-alpha12 | Android Software Development Kit License |
| `com.google.android.gms:play-services-iid` | 17.0.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-location` | 21.4.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-phenotype` | 17.0.0 | Android Software Development Kit License |
| `com.google.android.gms:play-services-stats` | 17.0.2 | Android Software Development Kit License |
| `com.google.android.gms:play-services-tasks` | 18.4.1 | Android Software Development Kit License |
| `com.google.android.gms:play-services-vision` | 20.1.3 | Android Software Development Kit License |
| `com.google.android.gms:play-services-vision-common` | 19.1.3 | Android Software Development Kit License |
| `com.google.firebase:firebase-iid-interop` | 17.1.0 | Android Software Development Kit License |
| `com.google.firebase:firebase-measurement-connector` | 19.0.0 | Android Software Development Kit License |
| `com.google.mlkit:genai-schema` | 1.0.0-alpha1 | Android Software Development Kit License |
| `com.google.mlkit:common` | 18.11.0 | ML Kit Terms of Service, https://developers.google.com/ml-kit/terms |
| `com.google.mlkit:genai-common` | 1.0.0-beta4 | ML Kit Terms of Service |
| `com.google.mlkit:genai-prompt` | 1.0.0-beta4 | ML Kit Terms of Service |
| `com.google.android.play:core-common` | 2.0.4 | Play Core Software Development Kit Terms of Service, https://developer.android.com/guide/playcore/license |
| `com.google.android.play:feature-delivery` | 2.1.0 | Play Core Software Development Kit Terms of Service |
| `com.google.android.play:review` | 2.0.2 | Play Core Software Development Kit Terms of Service |

Note: the package metadata of `com.google.android.datatransport:transport-*` and `com.google.android.material:material` says Apache-2.0 (listed in section 4), while the Chromium credits show them with the Android Software Development Kit License Agreement text.

## 4. Other packaged libraries

From the release runtime dependency graph (`releaseRuntimeClasspath`). Licence as stated in each library's package metadata.

| Library | Version | Licence | Text |
|---|---|---|---|
| `androidx.activity:activity` | 1.8.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.annotation:annotation` | 1.8.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.annotation:annotation-experimental` | 1.4.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.annotation:annotation-jvm` | 1.8.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.appcompat:appcompat` | 1.7.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.appcompat:appcompat-resources` | 1.7.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.arch.core:core-common` | 2.2.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.arch.core:core-runtime` | 2.2.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.browser:browser` | 1.8.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.cardview:cardview` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.collection:collection` | 1.4.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.collection:collection-jvm` | 1.4.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.concurrent:concurrent-futures` | 1.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.constraintlayout:constraintlayout` | 2.2.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.constraintlayout:constraintlayout-core` | 1.1.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.coordinatorlayout:coordinatorlayout` | 1.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.core:core` | 1.16.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.core:core-ktx` | 1.16.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.core:core-viewtree` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.cursoradapter:cursoradapter` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.customview:customview` | 1.2.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-android` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-core` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-core-android` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-core-okio` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-core-okio-jvm` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-preferences` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-preferences-android` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-preferences-core` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-preferences-core-android` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.datastore:datastore-preferences-external-protobuf` | 1.1.7 | BSD-3-Clause | LICENSES/BSD-3-Clause.txt |
| `androidx.datastore:datastore-preferences-proto` | 1.1.7 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.documentfile:documentfile` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.drawerlayout:drawerlayout` | 1.1.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.dynamicanimation:dynamicanimation` | 1.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.emoji2:emoji2` | 1.3.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.emoji2:emoji2-views-helper` | 1.3.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.fragment:fragment` | 1.5.4 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.graphics:graphics-shapes` | 1.0.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.graphics:graphics-shapes-android` | 1.0.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.interpolator:interpolator` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.legacy:legacy-support-core-utils` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-common` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-livedata` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-livedata-core` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-process` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-runtime` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-viewmodel` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.lifecycle:lifecycle-viewmodel-savedstate` | 2.6.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.loader:loader` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.localbroadcastmanager:localbroadcastmanager` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.media:media` | 1.6.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.mediarouter:mediarouter` | 1.8.0-beta01 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.palette:palette` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.print:print` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.profileinstaller:profileinstaller` | 1.4.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.recyclerview:recyclerview` | 1.2.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.resourceinspection:resourceinspection-annotation` | 1.0.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.savedstate:savedstate` | 1.2.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.startup:startup-runtime` | 1.1.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.tracing:tracing` | 1.2.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.transition:transition` | 1.5.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.vectordrawable:vectordrawable` | 1.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.vectordrawable:vectordrawable-animated` | 1.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.versionedparcelable:versionedparcelable` | 1.1.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.viewpager:viewpager` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.viewpager2:viewpager2` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `androidx.window.extensions.core:core` | 1.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.airbnb.android:lottie` | 6.7.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.android.datatransport:transport-api` | 3.1.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.android.datatransport:transport-backend-cct` | 3.1.9 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.android.datatransport:transport-runtime` | 3.1.9 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.android.material:material` | 1.14.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.auto.service:auto-service-annotations` | 1.1.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.code.findbugs:jsr305` | 3.0.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.errorprone:error_prone_annotations` | 2.50.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-annotations` | 17.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-common` | 23.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-components` | 19.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-datatransport` | 18.2.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-encoders` | 17.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-encoders-json` | 18.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-encoders-proto` | 16.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-installations` | 19.1.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-installations-interop` | 17.3.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.firebase:firebase-messaging` | 25.1.3 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.guava:failureaccess` | 1.0.3 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.guava:guava` | 33.7.1-jre | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.guava:listenablefuture` | 9999.0-empty-to-avoid-conflict-with-guava | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.j2objc:j2objc-annotations` | 3.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.google.protobuf:protobuf-javalite` | 4.36.2 | BSD-3-Clause | LICENSES/BSD-3-Clause.txt |
| `com.squareup.okio:okio` | 3.4.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `com.squareup.okio:okio-jvm` | 3.4.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `javax.inject:javax.inject` | 1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains:annotations` | 23.0.0 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-android-extensions-runtime` | 1.9.22 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-bom` | 1.8.22 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-parcelize-runtime` | 1.9.22 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-stdlib` | 2.3.21 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-stdlib-common` | 2.3.21 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-stdlib-jdk7` | 1.8.22 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlin:kotlin-stdlib-jdk8` | 1.8.22 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-android` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-bom` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-core` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-core-jvm` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-guava` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-play-services` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jetbrains.kotlinx:kotlinx-coroutines-reactive` | 1.10.2 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.jspecify:jspecify` | 1.0.1 | Apache-2.0 | LICENSES/Apache-2.0.txt |
| `org.reactivestreams:reactive-streams` | 1.0.3 | CC0-1.0 | LICENSES/CC0-1.0.txt |

Some of these libraries ship their own notice files inside the APK, for example `META-INF/androidx/constraintlayout/constraintlayout-core/LICENSE.txt` and `META-INF/third_party_licenses/com.google.mlkit/genai-schema/third_party_licenses.txt`.

## 5. Trademarks in bundled resources

Resources contributed by the Cefrium SDK and Google Play services carry names of third-party marks (Google, Google "G", Chrome, Google Cast, Google Lens, the "Google Sans" font name). These marks belong to their owners and are not licensed by this repository. See `TRADEMARKS.md` for the Mouklis marks.
