# BizCraft Studio - Corporate Website

## Overview
BizCraft Studioの架空コーポレートサイト。中小企業・個人事業主向けに業務システム・HP・AIツールをオーダーメイドで開発する「ビジネス×クラフト」の制作スタジオのWebサイトです。

## Project Structure
```
/
├── index.html      # トップページ（ヒーロー、選ばれる理由、サービス一覧）
├── works.html      # 制作実績ページ（6件の実績カード）
├── voice.html      # お客様の声ページ（4件のテスティモニアル）
├── price.html      # 料金プランページ（3つのプラン）
├── about.html      # BizCraft Studioについて（代表メッセージ・プロフィール）
├── contact.html    # お問い合わせページ（フォームUI）
└── style.css       # 共通スタイルシート
```

## Technical Specifications

### Technology Stack
- **HTML5**: セマンティックタグを使用（header, main, section, footer, nav, form等）
- **CSS3**: Pure CSS（Flexbox, Grid, Animations, Media Queries）
- **No JavaScript**: すべてHTML+CSSのみで実装

### Design Specifications
- **カラースキーム**:
  - ベースカラー: ネイビー (#0F172A)
  - アクセントカラー: オレンジ/ゴールド (#F59E0B)
  - 背景: ホワイト (#FFFFFF)、薄いグレー (#F9FAFB)
- **タイポグラフィ中心**: 余白多め、洗練されたBtoBデザイン
- **レスポンシブ対応**: PC / タブレット / スマホ対応

### CSS Features
- **BEM風クラス命名規則**: `.header`, `.header__nav`, `.card`, `.card__title`等
- **CSSアニメーション**: @keyframes fadeInUp、hover時のscale/shadow効果
- **CSSのみハンバーガーメニュー**: checkbox + labelハックで実装

## Recent Changes

### 2025-11-19: Initial Implementation
- 6ページ構成の静的HTMLサイトを作成
- 共通ヘッダー・フッター実装（全ページ共通）
- CSSのみでハンバーガーメニューを実装（モバイル対応）
- レスポンシブデザイン完全対応
- CSS アニメーション実装（fadeInUp、hover効果）
- 静的サイト用のワークフロー設定（Python HTTP Server on port 5000）

## Development

### Running Locally
静的サイトは自動的にポート5000で起動します。

```bash
python -m http.server 5000
```

### File Structure
- すべてのHTMLファイルは共通のヘッダー・フッターを使用
- `style.css`は全ページで共通
- WordPress移植を想定したシンプルな構造

## User Preferences
なし（初回作成）

## Project Architecture

### Design Approach
- **AI/SaaS系の洗練されたデザイン**: aidealab.comを参考
- **職人感 × テクノロジー × 信頼感**: コンセプトの3本柱
- **モバイルファースト**: レスポンシブ対応必須
- **WordPress移植前提**: シンプルで依存の少ない構造

### CSS Architecture
- リセット・ベーススタイル
- CSSアニメーション定義
- レイアウト・コンテナ
- ヘッダー・ナビゲーション
- セクション・カードコンポーネント
- フォーム
- フッター
- レスポンシブメディアクエリ

### Navigation Structure
- ホーム（index.html）
- サービス（index.html#service - ページ内リンク）
- 実績（works.html）
- お客様の声（voice.html）
- 料金プラン（price.html）
- 会社情報（about.html）
- お問い合わせ（contact.html）

## Notes
- お問い合わせフォームの送信処理はダミー（実装されていません）
- プライバシーポリシーのリンクはダミー（#）
- 将来的にWordPressテーマへの移植を想定した設計
