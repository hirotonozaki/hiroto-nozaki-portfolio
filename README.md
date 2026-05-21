# Hiroto Nozaki — Portfolio

> **考えて、つくる。** Web Production / Front-end.

野崎大翔（Hiroto Nozaki）のポートフォリオハブサイト。
4本の架空案件（焼肉 黒耀／NOVA TECH CAREERS／NEXUS Inc./NOIR MEN'S CLINIC）の Live Site・ソースコード・企画書 PDF への玄関として機能します。

---

## 🔗 Live Site

| 種別 | URL |
|---|---|
| **本リポジトリ（プロフィールサイト）** | https://hirotonozaki.github.io/ |
| 作品①｜焼肉 黒耀 | https://hirotonozaki.github.io/yakiniku-kokuyou/ |
| 作品②｜NOVA TECH CAREERS | https://hirotonozaki.github.io/nova-tech-careers/ |
| 作品③｜NEXUS Inc. | https://hirotonozaki.github.io/nexus-portfolio-site/ |
| 作品④｜NOIR MEN'S CLINIC | （WordPress テーマ実装中・ローカル環境） |

---

## このサイトについて

採用ご担当者様に最短経路で 4 作品を見渡していただくための「玄関」として制作したハブサイトです。
**3 分でポートフォリオ全体を把握できる構造**を最優先に、各作品の Live Site・GitHub・企画書 PDF への 3 リンクを 1 画面に集約しました。

掲載作品はすべて **Practice Projects / Fictional Client Works**（架空クライアントを想定した自主制作）です。

---

## デザイン方針

「**Apple 風ミニマル × 制作会社らしい品位 × 編集デザインの読ませる文体**」を一つの方向に統合することを試みました。

| 領域 | 方針 |
|---|---|
| **Color** | 漆黒 `#0a0a0a` をベースに、極小面積のシャンパンゴールド `#c9a96e` をアクセントに限定使用 |
| **Typography** | 見出しに **Fraunces**（可変セリフ・editorial 感）、本文に **Noto Sans JP**、数値・タグに **JetBrains Mono** |
| **Spacing** | セクション間 `clamp(96px, 12vw, 160px)`。Apple 並みの呼吸感を確保 |
| **Motion** | フェード＋Y軸 20px 移動のみ。`cubic-bezier(0.16, 1, 0.3, 1)` で統一 |

---

## 実装ポイント

| 領域 | 対応 |
|---|---|
| **Semantic HTML** | `<header>` / `<main>` / `<section>` / `<article>` の適切な使用、JSON-LD (Person)、OGP / Twitter Card |
| **CSS Architecture** | CSS 変数 + FLOCSS 命名、`clamp()` で可変余白 |
| **Responsive** | 4ブレイクポイント（480 / 768 / 1024 / 1340）、モバイルファースト、タッチターゲット 44px+ |
| **Accessibility** | ARIA 属性、`aria-expanded` / `aria-controls`、Esc 閉じ、`:focus-visible`、`prefers-reduced-motion` |
| **JavaScript** | Vanilla JS / IIFE / IntersectionObserver / `requestAnimationFrame` スロットリング |
| **Performance** | OGP は PNG 72KB、Google Fonts `preconnect`、`<noscript>` フォールバック |
| **Quality** | インライン style **0**、`!important` 4箇所のみ（`prefers-reduced-motion` 内の正当な用途）、FIX パッチなし |

---

## ディレクトリ構成

```
hiroto-nozaki-portfolio/
├── index.html              # ハブページ（縦動線1枚）
├── README.md
├── css/
│   └── style.css
├── js/
│   └── script.js
└── assets/
    ├── images/
    │   ├── ogp.png             # 1200×630 OGP/Twitter Card
    │   ├── noir-mockup.svg     # NOIR MEN'S CLINIC デザインモックアップ
    │   └── noir-wp-structure.svg # NOIR WordPress テーマ構造図
    └── pdf/
        ├── resume.pdf          # 履歴書（個人情報マスク版）
        ├── yakiniku-kokuyou-proposal.pdf
        ├── nova-tech-careers-proposal.pdf
        ├── nexus-proposal.pdf
        └── noir-mens-clinic-proposal.pdf
```

---

## 制作者情報

| 項目 | 内容 |
|---|---|
| Name | 野崎大翔（Hiroto Nozaki） |
| Role | Web Production / Front-end |
| Currently Learning | WordPress テーマ開発 / アクセシビリティ / パフォーマンス最適化 / Sass |
| GitHub | [github.com/hirotonozaki](https://github.com/hirotonozaki) |

---

<sub>本リポジトリ掲載の制作物はすべて架空企業を題材としたポートフォリオ作品です。</sub>
