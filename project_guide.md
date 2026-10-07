# Project Guide

本プロジェクトの文書の読み方を示す。

---

## 全体像

本プロジェクトは、以下の段取りで進める。

```
ビジネス設計 → 計測設計 → データ基盤 → 集計 → 分析・改善
```

| 段階 | 内容 | 状況 |
|---|---|---|
| ビジネス設計 | ビジネスゴール、ファネル、サイトの構造を定める | 完了 |
| 計測設計 | ファネルの各フェーズでのユーザー行動を、どのデータでどう判定するかを定める | 進行中 |
| データ基盤 | GA4・GSC・BigQuery を用いて、サイトから発生する行動ログデータを分析できる形に整える | 未着手 |
| 集計 | 計測設計とデータ基盤をもとに、生成されたデータから各種指標を算出する | 未着手 |
| 分析・改善 | 指標を用いて戦略を評価したり、施策を実施しその効果を検証することで、改善に繋げる | 未着手 |

## 文書の構成

```
docs/
└─ business_design/
   ├─ media_business_design.md
   ├─ site_design.md
   ├─ article_structure.md
   └─ site_navigation.md
```

## まず読む文書
| 文書 | 内容 |
|---|---|
|[media_business_design.md](docs/business_design/media_business_design.md) | ビジネスゴールと、それに至るファネル|

## 必要に応じて参照する文書

| 文書 | 内容 |
|---|---|
| [site_design.md](docs/business_design/site_design.md) | サイトの立ち位置、サイト構造、カテゴリ、URL、運営ポリシー |
| [article_structure.md](docs/business_design/article_structure.md) | 全記事に共通する4セクション(introduction・main・reference・cta) |
| [site_navigation.md](docs/business_design/site_navigation.md) | ページ同士の導線 |
