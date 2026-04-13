# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

myxyy.github.io — GitHub Pagesでホストされる個人ポートフォリオサイト（日本語）。
VRChat関連の3Dモデル、シェーダー作品、ワールド、イベント出展などを紹介している。

## 技術スタック

- ビルドツール・フレームワークなし。素のHTML + CSS のみ
- GitHub Pagesで直接配信（ビルドステップ不要）
- 依存パッケージなし（package.json, Gemfile 等は存在しない）

## ファイル構成

- `index.html` — サイト全体の唯一のページ
- `index.css` — 画像サイズ制御用のスタイル（セクションごとにクラスで管理）
- `img/` — ポートフォリオ用の画像アセット

## 開発方法

ビルド不要。`index.html` をブラウザで直接開くか、ローカルサーバーで確認する。

## コンテンツ構造（index.html）

HTMLは以下のセクション順で構成されている：
1. id（自己紹介）
2. 近影（VRChatアバター）
3. 興味の対象
4. 連絡先
5. つくったもの — 3Dモデル (`.avatars`)、シェーダー関連 (`.shaders`)、VRChatワールド (`.VRCWorlds`)、イベント出展 (`.events`)
6. 各種リンク

CSSクラス名（`.avatars`, `.shaders`, `.VRCWorlds`, `.events`）がセクション区分と対応している。

## 注意点

- コンテンツは全て日本語。コミットメッセージも日本語で書くこと
- 外部リンク（BOOTH, Twitter, VRChat起動リンク等）が多数含まれる。リンク切れに注意
- Twitter埋め込み (`blockquote.twitter-tweet`) を複数箇所で使用している
