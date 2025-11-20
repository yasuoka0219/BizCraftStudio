# BizCraft Studio - Corporate Website

## Overview
BizCraft Studioの架空コーポレートサイト。中小企業・個人事業主向けに業務システム・HP・AIツールをオーダーメイドで開発する「ビジネス×クラフト」の制作スタジオのWebサイトです。

## Project Structure
```
/
├── index.html           # トップページ（ヒーロー、選ばれる理由、サービス一覧）
├── service-system.html  # サービス詳細：業務システム開発（CRM・SFA・業務管理）
├── service-website.html # サービス詳細：ホームページ制作
├── service-ai.html      # サービス詳細：AIツール構築・業務自動化
├── works.html           # 制作実績ページ（6件の実績カード）
├── voice.html           # お客様の声ページ（4件のテスティモニアル）
├── price.html           # 料金プランページ（3つのプラン）
├── about.html           # BizCraft Studioについて（代表メッセージ・プロフィール）
├── contact.html         # お問い合わせページ（フォームUI）
└── style.css            # 共通スタイルシート
```

## Technical Specifications

### Technology Stack
- **HTML5**: セマンティックタグを使用（header, main, section, footer, nav, form等）
- **CSS3**: Pure CSS（Flexbox, Grid, Animations, Media Queries）
- **No JavaScript**: すべてHTML+CSSのみで実装

### Design Specifications
- **カラースキーム（ダーク系テクノロジーデザイン）**:
  - ベースカラー: ダークブルー/ブラック (#0A0E27, #0F172A, #1E293B)
  - アクセントカラー: シアン/ライトブルー (#00D9FF, #38BDF8)
  - テキスト: ホワイト/ライトグレー (#FFFFFF, #E2E8F0, #CBD5E1)
  - 背景画像: データビジュアライゼーション風の青い渦巻き（ヒーローセクション）
- **ダークモードデザイン**: サイバー/テクノロジー感のある洗練されたデザイン
- **レスポンシブ対応**: PC / タブレット / スマホ対応

### CSS Features
- **BEM風クラス命名規則**: `.header`, `.header__nav`, `.card`, `.card__title`等
- **CSSアニメーション**: @keyframes fadeInUp、float、pulse、shimmer等の多彩なアニメーション
- **CSSのみハンバーガーメニュー**: checkbox + labelハックで実装
- **グラデーション効果**: 背景、ボタン、カードアイコン、ラベル等に美しいグラデーション適用
- **CSS擬似要素アイコン**: 絵文字とCSS擬似要素（::before、::after）で視覚的要素を実装

### Visual Design Features
- **装飾的背景要素**: radial-gradientで作成した浮遊する円形要素（floatアニメーション）
- **グラデーションボーダー**: カードや実績カードに動的なグラデーション効果
- **絵文字アイコン**: ⚡💡👥🤖🎨📧等、視覚的な補助として各所に配置
- **ホバーエフェクト**: カード、ボタン、リンクに洗練されたトランジション効果
- **シャドウ効果**: 立体感と深みを演出する多層的なシャドウデザイン
- **3D球体要素**: ヒーローセクション右側に配置された3つの球体（三角形配置）

## Recent Changes

### 2025-11-20: Service Detail Pages Addition
- **3つのサービス詳細ページを追加**:
  - service-system.html: 業務システム開発（CRM・SFA・業務管理）の詳細ページ
  - service-website.html: ホームページ制作の詳細ページ
  - service-ai.html: AIツール構築・業務自動化の詳細ページ
- **各詳細ページの構成**:
  - page-hero（ページヒーロー）
  - サービス概要セクション
  - BizCraft Studioの強み（strength-list）
  - 解決できること・できることの例（usecase-list）
  - 提供機能・制作できるサイトの種類（feature-list）
  - サービスの流れ（flow-steps: 8ステップ図解）
  - 導入効果・成果イメージ（before-after-grid）
  - FAQ（faq-list）
  - CTAセクション
- **新規CSSコンポーネント追加**:
  - page-hero: 詳細ページ用ヒーローセクション
  - flow-steps / flow-step: サービスの流れのステップ表示
  - faq-list / faq-item: FAQ表示
  - feature-list / feature-item: 機能・特徴リスト
  - before-after-grid / before-after-card: Before/After比較カード
  - strength-list / strength-item: 強みリスト（横並び・アイコン付き）
  - usecase-list / usecase-item: ユースケース・解決できることリスト
  - service-card__link: サービスカードの「詳しく見る」リンク
- **トップページ（index.html）の更新**:
  - サービスカードに「詳しく見る →」リンクを追加
  - 各サービス詳細ページへの導線を実装
- **デザインの統一性**:
  - 既存のダーク系テクノロジーデザインを完全に維持
  - 青/シアンのグラデーション、グロー効果を全ページで統一
  - 既存のBEM風クラス命名規則を踏襲
  - hover効果、アニメーション、トランジションも既存と統一

### 2025-11-20: CTA Section Addition
- **お問い合わせCTAセクションを追加**:
  - サービスセクションとフッターの間に新しいCTAセクションを挿入
  - タイトル「Contact」、サブタイトル「● お問い合わせ」
  - 説明文：業務システム・AI活用・Webサイトのオーダーメイド開発を訴求
  - contact.htmlへのリンクボタン「お問い合わせはこちら」
- **ダーク系テクノロジーデザイン**:
  - 背景：ダークブルーのグラデーション（#0A0E27 → #0F172A → #1E293B）
  - 装飾的背景：radial-gradientで青/シアン系の微かなグロー効果
  - タイトル：3rem、シアンのtext-shadow
  - ボタン：青/シアンのグラデーション、ホワイトシャイン、hover時上昇＋拡大効果
- **レスポンシブ対応**:
  - デスクトップ（769px以上）: padding 6rem、タイトル 3rem
  - タブレット（481px-768px）: padding 4rem、タイトル 2.2rem
  - モバイル（480px以下）: padding 3rem、タイトル 1.8rem
- **自然な日本語コピー**:
  - サービス範囲を明示（業務システム・AI活用・Webサイト）
  - 具体的なサービス内容を列挙（課題整理、システム化、AIツール導入、サイト制作）
  - アーキテクトレビューで複数回改善し、自然な表現に仕上げ

### 2025-11-20: Reasons Section Expansion to 5 Items
- **選ばれる理由セクションを5つに拡張**:
  - 01: 完全オーダーメイドのシステム設計
  - 02: 中小企業・個人事業主に特化した開発スタイル
  - 03: 課題ヒアリングから改善提案まで伴走
  - 04: AI × 自動化で最大限の効率化
  - 05: CRM・勤怠・HP・AIまで幅広く対応できる柔軟性
- **横並びレイアウト（番号・テキスト・画像）**:
  - 大きな薄い青色の番号を左側に配置（5rem、rgba(56, 189, 248, 0.15)）
  - 中央にタイトルと説明文、右側に画像を配置
  - 奇数/偶数で背景色を変化させる
  - hover効果: 背景色の変化、画像の拡大（scale: 1.05）
- **AI生成画像5つ**:
  - images/reason-custom.png: カスタムシステム設計のビジュアライゼーション
  - images/reason-smallbiz.png: 中小企業向けワークスペース
  - images/reason-consulting.png: ビジネスコンサルティング
  - images/reason-ai.png: AIアルゴリズム開発
  - images/reason-system.png: システム開発コード画面
- **レスポンシブ対応**:
  - デスクトップ（769px以上）: 横並びレイアウト
  - タブレット（481px-768px）: 縦並びレイアウト、中央揃え
  - モバイル（480px以下）: 縦並びレイアウト、小さめフォント（番号2.8rem、タイトル1.1rem、テキスト0.85rem）

### 2025-11-20: Service Section Redesign with AI-Generated Images
- **サービスセクションのデザインリニューアル**:
  - AI生成画像を使用した3つのサービスカード（CRM、Web制作、AI自動化）
  - 画像上部・テキスト下部のカードレイアウトに変更
  - ダーク背景（section--dark）に白いカード（service-card）を配置
  - ホログラフィック・インターフェース風のテクノロジー画像
  - 青/シアン系のビジュアルでサイト全体のトンマナに統一
- **レスポンシブグリッドレイアウト**:
  - デスクトップ（769px以上）: 3列グリッド（auto-fit）
  - タブレット（481px-768px）: 2列グリッド（明示的指定）
  - モバイル（480px以下）: 1列グリッド
  - hover効果: カード上昇 + 画像拡大アニメーション
- **画像アセット追加**:
  - images/service-crm.png: CRMシステムのホログラフィック画像
  - images/service-web.png: Web制作のテクノロジー画像
  - images/service-ai.png: AI自動化のネットワーク画像

### 2025-11-20: Hero Section Orb Design Update
- **ファーストビュー右側BOXのデザイン変更**: 
  - 従来の縦並びカードから3つの球体（Orb）デザインに変更
  - 三角形配置（01: 業務システム開発、02: AI自動化、03: HP・LP制作）
  - radial-gradientで立体感のある球体表現
  - シアン/ブルー系のグロー効果（box-shadow複数層）
  - 浮遊アニメーション（float-center、float-normal）
  - hover時のscale効果とグロー強化（animation: none + transform: scale(1.08)）
  - 右側配置（margin-right: -50px）でより右寄りに表示
  - レスポンシブ対応（PC: 240px、タブレット: 180px、モバイル: 160px）

### 2025-11-20: Dark Tech Design Transformation
- **ダークモード化**: 全体をダーク系テクノロジーデザインに変更
  - カラースキームを黒/濃紺ベース、シアン/ブルーアクセントに変更
  - ヒーローセクションに青い渦巻きのデータビジュアライゼーション背景画像を追加
  - すべてのカード・セクションを半透明ダークカラーに変更
  - グラデーション効果を青/シアン系に統一
  - グロー・シャドウ効果でサイバー感を演出
  - すべてのHTMLファイルにキャッシュ制御metaタグを追加
  - CSSリンクにバージョンパラメータを追加してキャッシュ問題を解決

### 2025-11-19: Enhanced Visual Design
- **デザイン性大幅向上**: CSSのみで実装した視覚的要素を追加
  - グラデーション背景（ホワイト→グレー→ゴールド）
  - ヘッダーロゴに稲妻アイコン⚡追加
  - 絵文字アイコン（💡👥🤖🎨📧等）を各セクションに配置
  - カードにグラデーション効果とホバーアニメーション追加
  - セクションタイトル下にオレンジのアクセントライン追加
  - 実績カードにシマーアニメーション効果追加
  - floatアニメーション（浮遊効果）の装飾要素を追加
  - チェックマークアイコン付きリスト項目のデザイン改善

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
  - 業務システム開発（service-system.html）
  - ホームページ制作（service-website.html）
  - AIツール構築（service-ai.html）
- 実績（works.html）
- お客様の声（voice.html）
- 料金プラン（price.html）
- 会社情報（about.html）
- お問い合わせ（contact.html）

## Notes
- お問い合わせフォームの送信処理はダミー（実装されていません）
- プライバシーポリシーのリンクはダミー（#）
- 将来的にWordPressテーマへの移植を想定した設計
