# BizCraft Studio - Corporate Website

## Overview
BizCraft Studio is a fictional corporate website for a production studio specializing in bespoke business systems, websites, and AI tools for small to medium-sized businesses and sole proprietors. The project aims to showcase a "business x craft" approach to development, offering tailored solutions to clients. The business vision is to provide high-quality, customized digital solutions, focusing on AI/SaaS aesthetics and modern technology to build trust and demonstrate craftsmanship.

## User Preferences
I prefer detailed explanations.
I want iterative development.
Ask before making major changes.

## System Architecture

### UI/UX Decisions
The design adopts a dark, technology-themed aesthetic, inspired by AI/SaaS interfaces (e.g., aidealab.com).
- **Color Scheme**: Primarily dark blue/black (`#0A0E27`, `#0F172A`, `#1E293B`) with cyan/light blue accents (`#00D9FF`, `#38BDF8`). Text is white/light gray.
- **Visual Elements**: Features include data visualization-style background images (blue swirl in hero), floating circular elements with radial gradients, gradient borders, emoji icons for visual cues, and 3D spherical elements in the hero section.
- **Interactivity**: Extensive CSS animations (fadeInUp, float, pulse, shimmer), hover effects with transitions, and multi-layered shadow designs are used.
- **Responsiveness**: Fully responsive across PC, tablet, and mobile, with a mobile-first approach.

### Technical Implementations
- **Technology Stack**: Pure HTML5 and CSS3. No JavaScript is used for any interactive elements, including a CSS-only hamburger menu implemented via checkbox + label hack.
- **CSS Architecture**: Organized with a BEM-like naming convention (e.g., `.header`, `.card__title`). Includes sections for reset/base styles, animations, layout, header/navigation, components, forms, and media queries.
- **CSS Features**: Utilizes Flexbox and Grid for layout, `@keyframes` for animations, and CSS pseudo-elements (`::before`, `::after`) for iconography and decorative elements. Gradient effects are extensively used on backgrounds, buttons, and icons.

### Feature Specifications
- **Core Pages**: `index.html` (hero, reasons, services), `service-system.html`, `service-website.html`, `service-ai.html` (detailed service pages), `works.html` (portfolio), `voice.html` (testimonials), `price.html`, `about.html`, `contact.html`.
- **Service Flow**: Simplified 4-step process for System/Website development and a 3-step process for AI tool development.
- **Dynamic Elements**: Reasons section expanded to 5 items with AI-generated images and responsive layouts. Service section redesigned with AI-generated holographic interface-style images and responsive grid.
- **CTA**: A prominent Call-to-Action section is included between the service section and footer.
- **Navigation**: Comprehensive navigation linking to all main sections and detailed service pages.

### System Design Choices
- **Static Site**: Implemented as a static HTML site, intended for future migration to a WordPress theme, thus maintaining a simple and dependency-free structure.
- **File Structure**: Organized with a dedicated `style.css` for global styles and individual HTML files for each page.
- **Accessibility**: Semantic HTML5 tags are used throughout the structure.

## External Dependencies
None. The project is built using pure HTML and CSS with no external libraries, frameworks, or third-party services integrated.

## Recent Changes

### 2025-12-30: Case Studies Slider & Column Navigation
- **導入事例スライダーセクション追加（index.html）**:
  - サービスセクションとCTAセクションの間にスライド式導入事例セクションを追加
  - CSS scroll-snapを使用したJavaScript不要の横スクロールスライダー
  - 5件の事例カード（製造業A社、サービス業B社、EC事業C社、飲食チェーンD社、コンサル会社E社）
  - 各カードに: Case番号、企業名、写真、成果タイトル、業種タグ（色分け）、担当者名、ハッシュタグ
  - 新CSSクラス: .case-slider-section, .case-slide, .case-slide__header/company/image/title/footer等
- **コラム機能実装**:
  - column.html: コラム一覧ページ（カテゴリタブ、3カラムグリッド、ページネーション）
  - column/inside-sales-basics.html: インサイドセールス基礎記事
  - column/crm-introduction-guide.html: CRM導入ガイド記事
  - column/ai-business-automation.html: AI業務自動化記事
  - 全ページのナビゲーションに「コラム」リンクを追加（会社情報とお問い合わせの間）
  - 新CSSクラス: .column-grid, .column-card, .article-toc, .category-tabs等

### 2025-12-30: Service Feature Detail Pages Creation
- **4つの記事LPページ新規作成**: crm-sfa.htmlと同じデザインパターン
  - **ma-tool.html**: MAツール（マーケティングオートメーション）詳細ページ
  - **sns-auto.html**: SNS自動投稿システム詳細ページ
  - **ai-article.html**: AI記事制作サービス詳細ページ
  - **custom-solution.html**: オーダーメイドソリューション開発詳細ページ
- **共通構成**: ヒーロー → 共感セクション → 問題リスト → BizCraft Studioの強み（2x2グリッド）→ 中間CTA → FAQ → まとめ → 最終CTA
- **SEO対応**: 各ページにmeta description, OGP, FAQPage構造化データ（JSON-LD）
- **リンク設定**: service-system.htmlの「提供できる機能例」セクションから全5ページへのリンク

### 2025-12-30: CRM/SFA Article LP Page Creation
- **crm-sfa.html新規作成**: SEO最適化された記事型ランディングページ
  - **構成**: 共感→課題→なぜ問題が起きるのか→BizCraft Studioの強み→中間CTA→選ばれる理由→FAQ→まとめ
  - **SEO対応**: meta description, OGP, FAQPage構造化データ（JSON-LD）
  - **ビジュアル説明セクション**: 
    - 「なぜ問題が起きるのか」: 図解画像（data_chaos_infographic_diagram.png）+ ポイントカード形式
    - 「BizCraft Studioの強み」: 図解画像（unified_crm_solution_diagram.png）+ ポイントカード形式
  - **新CSSクラス**: .visual-explanation, .point-card, .article-content, .cta-card等
- **リンク追加**: 
  - service-system.html: 顧客管理システムをクリックでcrm-sfa.htmlへ遷移
  - price.html: 顧客管理システムカードの「詳しく見る」ボタンからcrm-sfa.htmlへ

### 2025-12-07: Feature Section Image Conversion
- **機能例・サイト種類セクションの画像化**:
  - **service-system.html「提供できる機能例」セクション**:
    - 絵文字アイコンからAI生成画像に差し替え
    - CRM / SFA → crm_sales_management_dashboard.png
    - KPIダッシュボード → kpi_analytics_dashboard.png
    - 勤怠 / シフト管理 → shift_attendance_management_system.png
    - 見積・契約・請求管理 → invoice_contract_management.png
    - 在庫管理 → inventory_warehouse_management.png
    - 通知・リマインド機能 → notification_reminder_alerts.png
  - **service-website.html「制作できるサイトの種類」セクション**:
    - 絵文字アイコンからAI生成画像に差し替え
    - コーポレートサイト → corporate_business_website.png
    - サービスサイト → service_product_website.png
    - LP（ランディングページ） → landing_page_design.png
    - 採用サイト → recruitment_career_website.png
    - ブログ・実績ページ付きサイト → blog_portfolio_website.png
    - ECサイト → e-commerce_online_store.png
  - **CSSクラス追加**: `.feature-item__image`（140px高さ、角丸、ホバーエフェクト）
  - **レスポンシブ対応**: object-fit: coverで画像をカバー表示

### 2025-12-07: Testimonial Images Update & Square Cropping
- **お客様の声セクションの画像差し替え**:
  - **新画像**: Gemini生成の4枚のビジネス写真に差し替え
    - 1. ミーティングシーン（製造業B社）
    - 2. カフェで電話する女性（サービス業C社）
    - 3. 自宅作業のデザイナー（EC事業D社）
    - 4. 飲食店の店長（飲食チェーンE社）
  - **正方形トリミング**: 
    - PC: 280x280px
    - モバイル: 200x200px
  - **object-position**: center topで顔が見切れないよう調整
  - **適用ページ**: voice.html、service-system.html、service-website.html、service-ai.html
  - **CSSバージョン**: v=20251207に統一

### 2025-12-06: Testimonial Spotlight Light Theme Redesign
- **お客様の声セクションのライトテーマへ変更**:
  - **背景**: ダーク→ライトグレー（rgba(241, 245, 249, 0.95)）に変更
  - **新要素**:
    - `testimonial-spotlight__title`: 大きなヘッドラインタイトル（数値部分を青色strong強調）
    - KPIボックス: 青い枠線（2px solid #00D9FF）のボックスデザイン
    - 商材・期間アイコン: 📦（--product）、📅（--period）を::before疑似要素で追加
  - **テキストカラー**: 白→ダークグレー（#1e293b / #475569）
  - **適用ページ**: voice.html、service-system.html、service-website.html、service-ai.html
  - **CSSバージョン**: 全ページをv=20251206に統一

### 2025-11-20: Testimonial Spotlight Initial Design
- **お客様の声セクションの全面リニューアル**:
  - **新しいデザイン形式**: 従来の小さなカードから大きなスポットライト形式に変更
  - **レイアウト**: 
    - PC: 左側40%（会社情報、業種タグ、KPI、商材・期間、詳細説明）、右側60%（人物写真）
    - モバイル: 縦並び（写真上、コンテンツ下）
  - **ビジュアル要素**:
    - 業種タグ（青いピル型バッジ）
    - KPI強調ブロック（オレンジグラデーション、大きな数値）
    - 淡い青/グレーのグラデーション背景
    - ビジネスポートレート写真（6枚のストック画像）
  - **適用ページ**:
    - service-system.html: 「導入効果イメージ」→「お客様の声」（製造業B社の事例）
    - service-website.html: 「成果イメージ」→「お客様の声」（サービス業C社の事例）
    - service-ai.html: 「導入効果イメージ」→「お客様の声」（EC事業D社の事例）
    - voice.html: 4件のお客様の声（B社、C社、D社、E社）
  - **CSSクラス**: testimonial-spotlight（メインコンテナ）、testimonial-spotlight__content、testimonial-spotlight__media、testimonial-spotlight__kpi（KPI強調）、testimonial-spotlight__tags（業種タグ）
  - **レスポンシブ**: ≤768pxでフレックスからカラムレイアウトに変更、画像アスペクト比調整

### 2025-11-20: Section Removal
- **不要なセクションの削除**:
  - service-system.html から「解決できること」セクションを削除
  - service-ai.html から「できることの例」セクションを削除
- **目的**: コンテンツの整理・簡素化

### 2025-11-20: Service Flow Visual Redesign
- **「サービスの流れ」セクションのビジュアルデザイン変更**:
  - **新デザイン**: 画像左・テキスト右のレイアウト（参考画像に基づく）
  - **ストック画像追加**: 各ステップに対応するビジネス写真を9枚取得
    - business_meeting_con_6813ae6d.jpg: ヒアリング・相談シーン
    - business_planning_de_21d9317b.jpg: 計画・設計シーン
    - software_development_81ddebf7.jpg: 開発・コーディングシーン
    - business_handshake_d_433cbeba.jpg: 契約・握手シーン
    - web_design_creative__f9ac8c4b.jpg: Webデザイン制作シーン
    - website_launch_celeb_59dd9cc7.jpg: サイト公開・祝賀シーン
    - business_analysis_da_6f475cfa.jpg: ビジネス分析シーン
    - ai_artificial_intell_89b0b8b3.jpg: AI開発シーン
    - software_testing_qua_8c2fc786.jpg: ソフトウェアテストシーン
  - **CSSの変更**:
    - flow-stepを2列グリッドレイアウト（画像40%、テキスト60%）に変更
    - flow-step__imageを追加（角丸、hover時拡大効果）
    - flow-step__badgeを追加（青いグラデーションバッジ "STEP 01"形式）
    - flow-step__contentを追加（テキストコンテンツのラッパー）
    - ステップ間に青い下向き矢印（▼）を追加
    - 淡い青/グレーの背景（rgba(226, 232, 240, 0.08)）
  - **レスポンシブ対応**:
    - PC（769px以上）: 画像左・テキスト右の2列レイアウト
    - タブレット・モバイル（768px以下）: 画像上・テキスト下の1列レイアウト
  - **適用ページ**: service-system.html（4STEP）、service-website.html（4STEP）、service-ai.html（3STEP）
- **パフォーマンス最適化**: すべての画像に`loading="lazy"`を追加