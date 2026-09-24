# FloatTone プライバシーポリシー / Privacy Policy

Language / 言語: [日本語 (Japanese)](#japanese) | [English](#english)

---

<h2 id="japanese">🇯🇵 日本語版 (Japanese)</h2>

最終更新日: 2026年9月24日

FloatTone（以下、「本アプリ」といいます。）は、ユーザーのプライバシーを尊重し、個人情報の保護に努めています。本プライバシーポリシーでは、本アプリにおける情報の取得、利用、管理、および保護について説明します。

### 1. 取得・アクセスする情報および利用目的

本アプリは、音楽再生およびライブラリ管理機能を提供するために、以下の情報にアクセスまたは利用します。

#### (1) 端末内の音声ファイルおよびストレージ情報
* **アクセス内容**: 端末ストレージ（内部ストレージおよびSDカード等）に保存されている音声ファイルおよびメタデータ（楽曲タイトル、アーティスト名、アルバム名、ジャケット画像等）。
* **利用目的**: 楽曲の再生、ライブラリ一覧の表示、プレイリスト作成、およびタグ情報の編集。
* **保存・送信**: これらのデータはすべてユーザーの端末内でのみ処理され、開発者の自作サーバーや第三者へ送信・収集されることは一切ありません。

#### (2) クラウドおよびネットワークストレージのアカウント・ファイル情報
* **対象サービス**: Google Drive、OneDrive、Dropbox、SMB (NAS)、WebDAV
* **アクセス内容**:
  * ユーザーの許可に基づくOAuth認証トークンおよびアクセス情報
  * 各ストレージ上に保存されている音声ファイルおよびそのメタデータ
* **利用目的**:
  * オンライン楽曲の再生および再生速度向上・データ通信量削減のための**一時キャッシュ保存**
  * ユーザーの明示的な操作による**端末ストレージへのダウンロード保存**
* **保存・管理**:
  * 認証トークンはユーザー端末内の安全な領域（ローカルストレージ）にのみ保存されます。
  * 接続処理およびファイル伝送は、開発者サーバーを経由せず、ユーザー端末と各サービス（またはユーザー所有のNAS/サーバー）間で直接行われます。

#### (3) アプリの診断・クラッシュ情報
* **利用ツール**: Google Firebase Crashlytics
* **アクセス内容**: アプリの不具合発生時に自動生成されるクラッシュレポート（スタックトレース、OSバージョン、端末モデル名、発生時刻等）。
* **利用目的**: アプリの不具合検出、原因調査、および動作安定性の向上。
* **個人特定**: 取得されるログは匿名化されており、個人を特定する情報（氏名、メールアドレス、電話番号等）は一切含まれません。

---

### 2. 外部SDKおよび第三者サービスの使用

本アプリでは、機能提供および品質維持のため、以下の第三者サービスおよびオープンソースライブラリを使用しています。

| サービス／ライブラリ名 | 提供元／分類 | 利用目的 |
| :--- | :--- | :--- |
| **Firebase Crashlytics** | Google LLC | アプリの不具合・クラッシュ解析 |
| **Google Play Services Auth / Drive API** | Google LLC | Google Drive への認証およびファイルアクセス |
| **Microsoft MSAL / Graph SDK** | Microsoft Corp. | OneDrive への認証およびファイルアクセス |
| **Dropbox SDK** | Dropbox, Inc. | Dropbox への認証およびファイルアクセス |
| **smbj** | オープンソース | ローカルネットワーク上の NAS (SMB) との直接通信 |
| **Sardine** | オープンソース | WebDAV サーバーとの直接通信 |
| **Android Jetpack Media3 (ExoPlayer)** | Google LLC | 音声ファイルの再生制御（端末内処理） |
| **jaudiotagger** | オープンソース | 楽曲タグ情報およびジャケット画像の端末内編集 |
| **Android Palette API** | Google LLC | アルバムアートからのカラー抽出およびUI表示補助 |

※本アプリには、広告配信SDKや行動追跡（トラッキング）用SDKは組み込まれておりません。

---

### 3. 情報の第三者提供および共有

本アプリは、法令に基づく場合を除き、取得したユーザー情報を第三者に販売、貸与、または提供することはありません。

---

### 4. データの削除および連携解除方法

ユーザーはいつでも自身のデータを管理・削除することができます。

1. **クラウドサービスの連携解除**:
   * 本アプリ内の設定画面より各クラウドサービスのアカウント連携を解除できます。解除を行うと、端末内に保存されていた認証トークンおよびキャッシュ情報は即座に削除されます。
   * 各クラウドサービス（Google、Microsoft、Dropbox 等）のアカウント管理画面から、本アプリのアクセス許可を取り消すことも可能です。
2. **ローカルキャッシュのクリア**:
   * アプリ内の設定画面より、一時保存された楽曲キャッシュを一括削除できます。
3. **アプリのアンインストール**:
   * アプリをアンインストールすることで、端末内に保持されているアプリ設定および認証情報はすべて削除されます。

---

### 5. 安全管理措置

本アプリは、情報の不正アクセス、紛失、改ざんを防止するため、以下のセキュリティ対策を実施しています。
* 通信の暗号化（HTTPS / TLS、SMB/WebDAVの安全なプロトコル）
* OAuth 2.0 に基づく安全なトークン認証
* 端末内ローカルストレージにおける認証情報の安全な保管

---

### 6. お問い合わせ窓口

本プライバシーポリシーまたは個人情報の取扱いに関するお問い合わせは、ストア掲載の開発者連絡先よりお願いいたします。

---
---

<h2 id="english">🇬🇧 English Version</h2>

Last Updated: September 24, 2026

FloatTone ("the App") respects user privacy and is committed to protecting personal information. This Privacy Policy explains how the App handles, accesses, and protects user information.

### 1. Information Accessed/Used and Purpose

The App accesses or uses the following information to provide music playback and library management features.

#### (1) On-Device Audio Files and Storage Information
* **Accessed Content**: Audio files and metadata (title, artist, album, cover artwork, etc.) stored in device storage (internal storage, SD card, etc.).
* **Purpose**: Music playback, displaying the music library, playlist creation, and audio tag editing.
* **Storage & Transmission**: All data is processed strictly locally on the user's device. No audio files or metadata are transmitted or collected by the developer or any third parties.

#### (2) Cloud & Network Storage Accounts and File Information
* **Supported Services**: Google Drive, OneDrive, Dropbox, SMB (NAS), WebDAV
* **Accessed Content**:
  * OAuth authentication tokens and access credentials granted with user permission.
  * Audio files and metadata stored in connected cloud/network storage.
* **Purpose**:
  * **Temporary Caching**: To stream online audio and temporarily cache files locally for faster playback and reduced data usage.
  * **Download to Device Storage**: To download files to local device storage upon explicit user action.
* **Storage & Management**:
  * Authentication tokens are stored securely in local device storage only.
  * File transfer and authentication occur directly between the user's device and the respective cloud provider (or local NAS/server), without passing through any developer servers.

#### (3) Diagnostic and Crash Information
* **Analytics Tool**: Google Firebase Crashlytics
* **Accessed Content**: Automatically generated crash reports when an error occurs (stack trace, OS version, device model, timestamp).
* **Purpose**: Detecting bugs, investigating crashes, and improving app stability.
* **Anonymity**: Collected data is strictly anonymized and contains no personally identifiable information (e.g., name, email address, phone number).

---

### 2. Third-Party Services and SDKs

The App uses the following third-party services and open-source libraries for functionality and quality maintenance.

| Service / Library | Provider / Type | Purpose |
| :--- | :--- | :--- |
| **Firebase Crashlytics** | Google LLC | App crash diagnostics and error logging |
| **Google Play Services Auth / Drive API** | Google LLC | Authentication and file access for Google Drive |
| **Microsoft MSAL / Graph SDK** | Microsoft Corp. | Authentication and file access for OneDrive |
| **Dropbox SDK** | Dropbox, Inc. | Authentication and file access for Dropbox |
| **smbj** | Open Source | Direct SMB connection for local network NAS |
| **Sardine** | Open Source | Direct WebDAV server connection |
| **Android Jetpack Media3 (ExoPlayer)** | Google LLC | Audio playback control (on-device) |
| **jaudiotagger** | Open Source | On-device editing of audio tags and artwork |
| **Android Palette API** | Google LLC | Extracting color themes from album artwork for UI |

*Note: The App contains no advertising SDKs or user tracking/behavioral analytics SDKs.*

---

### 3. Third-Party Data Disclosure and Sharing

Except as required by law, the App does not sell, rent, or share any user data with third parties.

---

### 4. Data Deletion and Account Disconnection

Users can manage or delete their data at any time:

1. **Disconnecting Cloud Services**:
   * Users can disconnect cloud service accounts at any time from the App's settings screen. Disconnecting immediately deletes local authentication tokens and cached files.
   * Permissions can also be revoked directly from the user's Google, Microsoft, or Dropbox account settings.
2. **Clearing Local Cache**:
   * Cached audio files can be cleared at once via the App's settings screen.
3. **Uninstalling the App**:
   * Uninstalling the App removes all app settings, cached data, and local credentials.

---

### 5. Security Measures

The App implements the following security measures to protect user data:
* Encrypted communications (HTTPS / TLS and secure network protocols for SMB/WebDAV)
* Secure OAuth 2.0 authentication
* Safe local storage of authentication tokens on device

---

### 6. Contact Us

If you have any questions regarding this Privacy Policy or data privacy, please contact us via the developer contact email listed on the Google Play Store page.
