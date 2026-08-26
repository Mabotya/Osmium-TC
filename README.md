# Osmium TC （旧TCSH）

Osmium TCは、**TRAIN CREW**の楽しみを拡張するためのサードパーティー製ソフトです。
音声ファイルの変換・配置を簡単に行えるほか、プリセット、音声編集、作曲、マイク放送、カスタムUI、車内LCDなどを利用できます。

> Osmium TCは非公式ツールです。  
> TRAIN CREW公式および関係各所とは一切関係ありません。

## ダウンロード

右側の「Releases」または以下のページから、最新版をダウンロードしてください。

**[最新版をダウンロード](../../releases/latest)**

## 主な機能

- カスタムサウンドに関する設定をより簡単に
- 作曲や編集した音声をTRAIN CREWへ簡単に反映
- 音声加工による臨場感のある肉声放送
- 様々な音声を入れられるタブレット放送
- より自由にカスタマイズできるUI
- API連動による車内LCD風表示

## Microsoft Defender SmartScreenについて

個人開発のWindows向けソフトのため、初回起動時にMicrosoft Defender SmartScreenの警告が表示される場合があります。

このGitHubリポジトリからダウンロードしたことを確認したうえで実行する場合は、  
**「詳細情報」→「実行」** を選択してください。

配布元を確認できない場合や、不安がある場合は実行しないでください。

## 注意事項

- TRAIN CREW側の仕様変更により、正常に動作しなくなる場合があります。
- API連動機能やカスタムUIは、TRAIN CREWから取得できる情報に依存します。
- 音声やプリセットを共有する際は、著作権や利用規約を確認してください。
- 本ソフトの使用によって発生した不具合やデータ損失について、開発者は責任を負いません。

## 不具合報告・要望

不具合や機能要望は、以下のページから送信できます。

**[Osmium TC 不具合報告・要望フォーム](https://o-nnect.com/tcsh%e5%a0%b1%e5%91%8a/)**

## 配布について

TCSH独自部分の無断転載、再配布、改変は禁止します。
ただし、TCSHに同梱されている第三者ソフトウェアには、それぞれのライセンスが適用されます。FFmpegにはGNU Lesser General Public License version 2.1以降が適用されます。

---

# Osmium TC (formerly TCSH)

Osmium TC is a third-party application designed to expand the **TRAIN CREW** experience.

It makes it easy to convert and manage audio files, and also provides features such as presets, audio editing, music composition, microphone announcements, custom UIs, and in-train LCD-style displays.

> Osmium TC is an unofficial tool.  
> It is not affiliated with or endorsed by TRAIN CREW or any related parties.

## Download

Download the latest version from the "Releases" section on the right side of this page, or from the link below.

**[Download the latest version](../../releases/latest)**

## Main Features

- Easier setup and management of custom sounds
- Easily apply composed or edited audio to TRAIN CREW
- Create more realistic microphone announcements with audio processing
- Tablet-style announcement system that can play various audio files
- More flexible and customizable UI
- In-train LCD-style displays using API integration

## About Microsoft Defender SmartScreen

Because Osmium TC is an independently developed Windows application, Microsoft Defender SmartScreen may display a warning when you launch it for the first time.

If you have confirmed that the application was downloaded from this GitHub repository and wish to run it, select:  
**"More info" → "Run anyway"**

If you cannot verify the source of the application or have any concerns, do not run it.

## Notes

- Changes to TRAIN CREW may cause some features to stop working correctly.
- API-based features and custom UIs depend on the information available from TRAIN CREW.
- When sharing audio files or presets, make sure to comply with applicable copyright laws and terms of use.
- The developer is not responsible for any issues or data loss resulting from the use of this software.

## Bug Reports & Feature Requests

You can report bugs or submit feature requests using the page below.

**[Osmium TC Bug Report & Feature Request Form](https://o-nnect.com/tcsh%e5%a0%b1%e5%91%8a/)**

## Redistribution

Unauthorized redistribution, modification, or republishing of TCSH-specific components is prohibited.

However, third-party software included with TCSH is subject to its respective license terms. FFmpeg is licensed under the GNU Lesser General Public License version 2.1 or later.

---

## FFmpegについて

TCSHには、動画ファイルから音声を抽出するため、FFmpeg 7.1のコマンドライン実行ファイルを同梱しています。

- ソフトウェア: FFmpeg 7.1
- 著作権: Copyright (c) 2000-2024 the FFmpeg developers
- ライセンス: GNU Lesser General Public License version 2.1 or later
- 利用方法: TCSHから独立した別プロセスとして実行
- ビルド環境: MSYS2 UCRT64
- 外部コーデックライブラリ: なし
- FFmpegソースコミット: `b08d7969c550a804a59511c7b83f2dd8cc0499b8`
- 同梱ffmpeg.exe SHA-256:  
  `40a415ec7b3c77cd1c62069459a8023e06d20af05aabd1cd08709a167c124097`

FFmpeg本体は改変せず、公式ソースコードからTCSH向けにビルドしています。
ビルド時は外部ライブラリの自動検出を無効化し、GPLまたは非自由ライセンスの外部コーデックライブラリをリンクしていません。

### ライセンス

- [FFmpeg公式サイト](https://ffmpeg.org/)
- [FFmpegソースリポジトリ](https://github.com/FFmpeg/FFmpeg)
- [GNU LGPL version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)

ライセンス全文は、TCSHに同梱されている
`tools/FFmpeg/LICENSE.txt`
にも収録しています。

### 対応ソースコード

TCSHに同梱している下記FFmpegバイナリに対応する完全なソースコードとビルド資料は、以下から取得できます。

- 対象ffmpeg.exe SHA-256:  
  `40a415ec7b3c77cd1c62069459a8023e06d20af05aabd1cd08709a167c124097`

[ffmpeg-7.1-tcsh-lgpl-corresponding-source.zip](https://github.com/Mabotya/TCSH/releases/download/v1.9.0/ffmpeg-7.1-tcsh-lgpl-corresponding-source.zip)

このZIPには以下を収録しています。

- 使用したFFmpeg 7.1の完全なソースコード
- 正確なconfigure設定
- ビルドスクリプト
- MSYS2パッケージ一覧
- ビルド手順
- ライセンス文書
