[English](README.md) · [中文](README.zh-CN.md) · **日本語** · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

<p align="center">
  <img src="docs/banner.svg" alt="ScsSubst" width="100%">
</p>

<h1 align="center">ScsSubst</h1>

<p align="center">
  <strong>フォルダをドライブレターに</strong><br>
  深いフォルダにドライブレターを。コピー不要、ローカルディスク感覚。
</p>

<p align="center">
  <a href="https://subst.scsoi.com"><img src="https://img.shields.io/badge/Website-subst.scsoi.com-0F766E?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scssubst/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scssubst?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://subst.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://subst.scsoi.com/#download"><strong>ダウンロード</strong></a> ·
  <a href="https://subst.scsoi.com/#pricing"><strong>料金</strong></a> ·
  <a href="https://github.com/shuyingegit/scssubst/releases"><strong>リリース</strong></a> ·
  <a href="https://drive.scsoi.com"><strong>ScsDriver</strong></a>
</p>

---

## ScsSubst を選ぶ理由

深いフォルダにドライブレターを。コピー不要、ローカルディスク感覚。

書き込み・削除ができるツールを使うとき、越境して誤削除されるのが怖い？出られない作業ドライブを。

<p align="center">
  <img src="docs/hero.png" alt="ScsSubst hero" width="920">
</p>

## こんな使い方

- よく使うフォルダ → ドライブレター
- ツールを1つのドライブに閉じ込める
- 長いプロジェクトパスを短縮
- 作業場所ごとにドライブを分ける

### 注目：より安全なサンドボックス作業ドライブ

**出られない作業ドライブを**

越境・誤削除が怖いなら、作業フォルダをドライブレターにしてツールをそこに閉じ込める。

1. 専用の作業フォルダを作る
2. ドライブレターに（例: Z:）
3. ツールの作業場所を Z: に

> ツールの作業場所をそのドライブに。実用的な隔離で、カーネル級サンドボックスではない。

<p align="center">
  <img src="docs/sandbox-usecase.png" alt="ScsSubst sandbox use case" width="920">
</p>

## 主な機能

シンプル、安定、手間いらず。

- **ワンクリックマウント** — フォルダとドライブレターを選び「接続」。起動時の自動マウントも可能。
- **ネイティブ体験** — エクスプローラーで普通のドライブと同じように使えます。
- **自動起動** — アプリ起動時に保存したマッピングを自動で戻せます。
- **軽量・安定** — Windows API のみ。サードパーティのファイルシステムドライバは不要。
- **複数マッピング** — 複数のフォルダマッピングを追加でき、それぞれ独立したドライブレター。
- **詳細オプション** — 管理者アプリから見える、ごみ箱など。既定はシンプル。
- **インストールですぐ試用** — 既定 7 日の試用。その後はライセンス（月／年／買い切り）で有効化。
- **サンドボックス作業ドライブ** — 書き込み系ツールはしばしば越境して誤削除する。専用フォルダをドライブレターにし、作業場所をそこに。はみ出しにくくなります。


## ダウンロード

最新ビルド: **[GitHub リリース](https://github.com/shuyingegit/scssubst/releases/latest)** · [公式サイト](https://subst.scsoi.com/#download)

| パッケージ | 用途 |
|--------|----------|
| **Portable (`.zip`)** | 解凍して実行（推奨） |
| **Installer (`.exe`)** | インストーラー |

動作環境：Windows 10 / 11（64ビット）

## 料金

無料トライアルは 7 日から。友達を招待すると、双方の試用を延長できます。

すべてのプラン（無料トライアル含む）に技術サポート付き。利用中にエラーや問題があればメールください。調査・修正し改善を続けます。

## 関連製品

WebDAV / ネットディスクを Windows のローカルドライブとしてマウント。

→ **[ScsDrive](https://github.com/shuyingegit/scsdriver)** · [drive.scsoi.com](https://drive.scsoi.com)

## よくある質問

**ScsSubst とクラウドマウントの違いは？**  
ScsSubst は PC 上の既存フォルダをマップします。WebDAV / ネットディスクは姉妹製品 ScsDriver（drive.scsoi.com）をご利用ください。

**トライアル版と製品版の違いは？**  
機能は同じです。トライアルは 7 日。友達の招待コードで始めると 14 日になります。あなたが招待した相手がトライアルを始めると、自分も +7 日（上限なし）。買い切り無期限は対象外。終了後はライセンスが必要です。

**ScsSubst で安全なサンドボックス作業ドライブを作るには？**  
専用フォルダを作りドライブレターにマップし、ツールの作業場所をそこに向けます。誤削除もそのドライブ内に収まります。OS 級サンドボックスではない点に注意。

## ライセンスと規約

利用規約 · プライバシーポリシー · 返金ポリシー — [https://subst.scsoi.com/terms](https://subst.scsoi.com/terms) · [https://subst.scsoi.com/privacy](https://subst.scsoi.com/privacy) · [https://subst.scsoi.com/refund](https://subst.scsoi.com/refund)

---

<p align="center">
  <a href="https://subst.scsoi.com/"><strong>公式サイトを開く →</strong></a>
</p>
