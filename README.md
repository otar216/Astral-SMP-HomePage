# Astral-SMP Official Website

Astral-SMPの公式Webサイトプロジェクト。
HTML/CSS/JSのみで構成。

## ディレクトリ構成
```text
/
 ├ index.html        (Homeページ)
 ├ contents.html     (Contentsページ: 建築紹介など)
 ├ history.html      (Historyページ: 沿革)
 ├ css/style.css     (デザイン全般のスタイル)
 ├ js/main.js        (ナビゲーション動作などのスクリプト)
 └ assets/
     ├ images/       (画像ファイル)
        └ contents/      (コンテンツ用の画像)
        └ members/      (鯖メンのアイコン用の画像)
        └ history/      (沿革用の画像)
     └ icons/        (SNSアイコン)
```

## 更新ガイド

### 画像の差し替え
`assets/images` フォルダ内の画像を同じファイル名で上書きするだけで反映されます。

- **背景画像**: `assets/images/home_bg.png` (推奨サイズ: 1920x1080以上)
- **コンテンツ画像**: `assets/images/contents/` 内のファイル
- **沿革画像**: `assets/images/history/` 内のファイル

### テキストの変更
各HTMLファイルをテキストエディタで開き、該当する文字を直接編集してください。
日本語が含まれている箇所が主に編集対象です。

### コンテンツの追加 (Contentsページ)
`contents.html` 内の `<article class="content-card">...</article>` のブロックをコピー＆ペーストし、画像パスとテキストを変更することで増やせます。

### 沿革の追加 (Historyページ)
`history.html` 内の `<div class="timeline-item">...</div>` のブロックをコピー＆ペーストして追加してください。
自動的に左右交互に配置されます。

## カラーテーマの変更
`css/style.css` の冒頭にある `:root` 内の変数を変更することで、サイト全体の色味を一括調整できます。
```css
:root {
  --color-bg-deep: #0f0f4d; /* メイン背景色 */
  --color-accent: #4d4dff; /* アクセントカラー */
  ...
}
```
