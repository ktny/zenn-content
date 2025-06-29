# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

このリポジトリはZenn（技術記事投稿プラットフォーム）用のコンテンツ管理リポジトリです。技術記事とブックを管理し、プレビュー機能を提供します。

## 開発環境

- Node.js: 17.5.0（Volta管理）
- npm: 8.4.1
- Zenn CLI: ^0.1.94

## 基本コマンド

### 記事作成
```bash
npm run create
# または
npx zenn new:article
```

### プレビュー
```bash
npm run preview
# または
npx zenn preview
```

## ディレクトリ構造

- `articles/`: 技術記事のMarkdownファイル
- `books/`: 本（ブック）のコンテンツ
- `package.json`: npm設定とスクリプト

## 記事ファイルの構造

各記事ファイルは以下のYAMLフロントマターを持ちます：

```yaml
---
title: "記事のタイトル"
emoji: "🐕"
type: "tech"  # tech: 技術記事 / idea: アイデア
topics: []
published: false  # 公開状態
---
```

## 開発時の注意事項

- 記事作成時は`published: false`で下書き状態として開始
- プレビューで内容を確認してから公開設定を変更
- 絵文字とトピックタグの設定を忘れずに行う