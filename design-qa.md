# ENISHI サイトのデザイン確認

- Source visual truth: アプリの `Screenshots/01-project-list.png`、`MarriageFormCreator/Assets.xcassets/AppIcon.appiconset/AppIcon.png`。
- Implementation: ホーム、プライバシーポリシー、利用規約、サポートの静的ページ。
- Scope: アプリのブランドをWebのサポートページへ適用する変更。アプリ画面そのものの複製ではない。Webのヒーローと目次は意図した構造差。
- Evidence in the private app repository: `Docs/PublicSiteDesign/home-desktop.jpg`, `home-mobile.jpg`, `privacy-mobile.jpg`, `terms-desktop.jpg`, `comparison.jpg`。
- Viewports: desktop 1280×960、mobile 390×844、small mobile 320×740 CSS px。ブラウザキャプチャは1 CSS pxあたり1画像px。アプリ参照1206×2622pxは幅390pxへ縮小して比較。アイコン参照1024×1024px。
- Full-view comparison: アプリ画面・アプリアイコン・Webホームを `comparison.jpg` 内で並べて確認。異なる画面のため、ピクセル単位の配置一致ではなくブランド適用を評価。
- Focused evidence: 規約本文とデスクトップ目次は `terms-desktop.jpg`、モバイル本文と折りたたみ目次は `privacy-mobile.jpg`、ロゴ・ヒーロー・カードはホームの個別キャプチャで確認。

## Findings

P0/P1/P2に該当する未解決事項なし。

- Typography: アプリ同様のシステムゴシック体を本文・ナビゲーション・カードに使用。ホームの見出しは婚礼向けの落ち着いた明朝体へ意図的に変更。本文14–15px、行高2.05、モバイルタイトル26px。切れ・重なりなし。
- Layout: アプリの角丸カードと余白を踏襲。デスクトップは3列カードと2列の文書レイアウト、モバイルは1列。320px・390px・1280pxで横方向のはみ出しなし。
- Colors: アイボリー #f6f2ed、白系カード #fffdf9、ワインレッド #80384b を使用。アプリの背景と赤系アクセントを適用。本文は濃い茶系 #332b29、補助文 #716665。
- Assets: 既存のENISHIアイコンをそのまま使用し、ヘッダー・ヒーロー・faviconへ展開。手描きやCSSによる模倣なし。欠損画像なし。
- Copy: 規約・プライバシー・サポートの元の本文、問い合わせ先 `cychow.app@gmail.com`、更新日は保持。ホームはアプリと同じ「ふたりのはじまりをふたりらしく」を採用。
- Interaction: ホームからプライバシーページへのリンク、モバイル目次の開閉・該当見出しへの移動、メールリンクを確認。全ページの内部リンクとアンカーを検証。ブラウザのコンソールエラーなし。
- Accessibility: 主見出し各1つ、本文スキップリンク、ナビゲーションラベル、選択中のページ表示、フォーカス表示、画像代替文、動きの軽減設定に対応。

## Comparison history

初回のブランド比較・デスクトップ・モバイル表示確認でP0/P1/P2なし。本文およびリンクの保持も確認。追加修正の反復は不要。

## Follow-up polish

追加のブランド変更時に、Webページの色とアプリアイコンを併せて更新する。

final result: passed
