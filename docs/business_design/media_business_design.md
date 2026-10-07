# Media Business Design

deepintoanalytics.com のビジネスゴールと、その達成に向けた戦略を定める。

---

## ビジネスゴール

> 自分のファンをつくる

「自分のファンをつくる」とは、サイト訪問者や X ユーザーが、次のいずれかの行動(ファン化行動)を起こすことと定める。

- 当サイト上の Stripe で投げ銭をする
- 自分の X アカウントをフォローする

---

## 戦略

### ファネルモデル

ビジネスゴールに至る典型的な関与の深化経路を、次の4フェーズで表す。

```
Attention → Consumption → Interest → Action
```

関与は、訪問者とコンテンツ・執筆者との関係の深さを指す概念であり、GA4 のエンゲージメント指標とは別物である。

共通規則:

- フェーズはセッション単位で判定する
- 各フェーズは、必ずしも順番に到達しない
- セッション内で一度到達したフェーズは、その後のページ遷移によって取り消さない
- ファネルが扱うのは、サイトを経由する経路のみとし、X 上で完結するファン化は、ファネルの外で生じる
- Books の閲覧はファネルの外とする
- Consumption の後、離脱して後続のセッションで再び Attention から入る経路(Return loop)がある。

ページとセクションの構成は [site_design.md](site_design.md)、[article_structure.md](article_structure.md)、[site_navigation.md](site_navigation.md) で定める。

### Attention

#### 定義

記事へ流入して、記事の main を読み始めるまで。

#### 期待する訪問者の状態

記事の存在を認識し、受け入れる。

#### 戦略

- SEO により、設定した検索キーワードで上位に表示させる。
- X で継続的に投稿する。
- 記事の introduction で、読者を main に引き込む。

対象とする読者は、[site_design.md](site_design.md) で定めたターゲット読者とする。

### Consumption

#### 定義

セッション内で最初に記事の main を読み始めた時点で Consumption のスタートとする(Attention の完了)。
スタート後の `/articles/` 内での閲覧、および他の記事への回遊も Consumption に含む。ただし、回遊先の記事で Attention には戻らない。

#### 期待する訪問者の状態

記事を有益だと評価する。

#### 戦略

[site_design.md](site_design.md) の USP に基づく記事を提供する。

#### Consumption の程度

Consumption には、訪問者が記事に認める価値の程度に応じたグラデーションが存在する。

Consumption に到達し、そのセッションでは Interest・Action に進まずに離脱したセッションを Spot Consumption Session と呼ぶ。Spot Consumption Session は失敗とはみなさない。ファン化は、複数回の訪問を通じて起こり得る。

### Interest

#### 定義

セッション内で profile または story に到達した時点で Interest に到達する。

#### 期待する訪問者の状態

執筆者自身へ関心が移る。

#### 戦略

- 記事の cta から profile へ、profile から story へと導く。
- profile で、運営者が何者で、何を目指し、何に取り組んでいるかを示す。
- story で、運営者の軌跡を語る。

#### Interest の程度

Interest には、訪問者が執筆者に向ける関心の深さに応じた程度が存在する。profile から story へと進むにつれて、関心が深まることを想定する。

### Action

#### 定義

ファン化行動を実行する。

#### 期待する訪問者の状態

ファンになる。

#### 戦略

X アカウントと投げ銭への導線を設ける。配置は [site_navigation.md](site_navigation.md) で定める。
