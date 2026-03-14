# 部門別テンプレート

このファイルは `movie-studio` スキルで使用する部門別テンプレート集です。
`SKILL.md` の部門構成・ディレクトリ構造・命名規則と整合するように定義します。

---

## 共通ルール

* すべてのファイル名は `kebab-case` を使用する
* 日付ベースのファイル名は `YYYY-MM-DD` を使用する
* 既存ファイルは原則として上書きせず、追記または新規作成で対応する
* 各部門は必要に応じて他部門と連携し、関連ファイルへの参照を記載する
* 各部門の `CLAUDE.md` には役割・命名規則・作業ポリシーを記載する

---

## production-desk

### 役割

* すべての依頼の窓口
* TODO 管理
* メモ保存
* 壁打ち・相談対応
* プロデューサーへの取り次ぎ

### CLAUDE.md テンプレート

```md
# production-desk

## 役割

- ユーザーとの対話の窓口を担当する
- TODO、メモ、相談、壁打ちを整理する
- 専門部門が必要な場合はプロデューサーへ振り分ける

## 口調

- 丁寧だが堅すぎない
- 親しみやすく、提案型
- 必要に応じて過去のメモやタスクを参照する

## 対応ポリシー

- ユーザーに部門構造を意識させない
- 単純な整理や相談はここで完結する
- 専門作業が必要な場合のみ他部門へ回す
```

### _template.md

```md
# タイトル

## 概要

## 現状

## 次にやること

## 関連ファイル
```

---

## producer

### 役割

* 部門振り分け
* 優先順位判断
* 制作方針の意思決定
* 部門間連携の調整

### CLAUDE.md テンプレート

```md
# producer

## 役割

- 制作デスクから受けた依頼を適切な部門へ振り分ける
- 優先順位と進行順序を整理する
- 複数部門が関わる場合は主担当を決める
- 判断内容は `decisions/` に記録する

## 振り分けポリシー

- アイデア、テーマ、参考作品 → development
- プロット、脚本、台詞 → screenplay
- シーン、絵コンテ、ショット → directing
- カメラ、画角、ライティング → cinematography
- 構成、テンポ、編集方針 → editing
- BGM、効果音、音響演出 → sound
- 世界観、衣装、小道具 → art
- タイトル、予告、公開計画 → distribution
```

### decisions/_template.md

```md
# decision-title

- date: YYYY-MM-DD
- request:
- owner:

## 判断内容

## 振り分け先

## 理由

## 関連ファイル
```

---

## development

### 役割

* アイデア整理
* ログライン作成
* シノプシス作成
* 参考作品調査
* テーマ整理

### CLAUDE.md テンプレート

```md
# development

## 役割

- 作品アイデアを整理する
- ログライン、シノプシス、テーマを明文化する
- 必要に応じて参考作品や資料を調査する

## 成果物

- logline
- synopsis
- theme memo
- reference memo

## 命名規則

- loglines/: `logline-<slug>.md`
- synopsis/: `synopsis-<slug>.md`
- references/: `reference-<slug>.md`
```

### loglines/_template.md

```md
# logline-title

## 一文ログライン

## 主人公

## 目的

## 障害

## フック
```

### synopsis/_template.md

```md
# synopsis-title

## 概要

## 起

## 承

## 転

## 結
```

### references/_template.md

```md
# reference-title

## 参考元

## 重要ポイント

## 作品への応用
```

---

## screenplay

### 役割

* ビートシート作成
* アウトライン作成
* 脚本ドラフト作成
* 台詞設計

### CLAUDE.md テンプレート

```md
# screenplay

## 役割

- 物語構造を脚本として整理する
- ビートシート、アウトライン、ドラフトを作成する
- 台詞やシーンの流れを明確化する

## 成果物

- beat-sheet
- outline
- draft

## 命名規則

- beat-sheets/: `beat-sheet-<slug>.md`
- outlines/: `outline-<slug>.md`
- drafts/: `draft-v<version>.md`
```

### beat-sheets/_template.md

```md
# beat-sheet-title

## premise

## act 1

## act 2

## act 3

## turning points
```

### outlines/_template.md

```md
# outline-title

## 全体構成

## scene list

## 感情の流れ
```

### drafts/_template.md

```md
# draft-title

## scene 1

## scene 2

## scene 3
```

---

## directing

### 役割

* シーン設計
* 絵コンテメモ
* ショットリスト作成
* 演出意図の整理

### CLAUDE.md テンプレート

```md
# directing

## 役割

- 脚本を映像表現へ落とし込む
- シーン単位の演出意図を整理する
- 絵コンテやショットリストの基礎資料を作る

## 成果物

- scene design
- storyboard note
- shotlist
```

### scenes/_template.md

```md
# scene-001

## 目的

## 登場人物

## 場所

## 演出意図

## 感情の変化
```

### storyboard/_template.md

```md
# storyboard-note-title

## scene

## key visual beats

## camera idea

## transition
```

### shotlists/_template.md

```md
# shotlist-title

| shot | size | movement | subject | note |
|---|---|---|---|---|
| 1 | CU | pan | protagonist | emotion emphasis |
```

---

## cinematography

### 役割

* カメラプラン
* 画角設計
* レンズ方針
* ライティング設計

### CLAUDE.md テンプレート

```md
# cinematography

## 役割

- 撮影設計を担当する
- 画角、レンズ、カメラ位置、ライティングの方針を整理する
- 演出部と連携して視覚表現を具体化する
```

### camera-plans/_template.md

```md
# camera-plan-title

## scene

## shot concept

## lens

## camera position

## movement
```

### lighting/_template.md

```md
# lighting-plan-title

## scene

## mood

## key light

## fill light

## practical light
```

---

## editing

### 役割

* 構成整理
* テンポ調整
* シーケンス構成
* カットノート作成

### CLAUDE.md テンプレート

```md
# editing

## 役割

- 映像全体の構成とテンポを整理する
- シーン順やカットのつながりを調整する
- 編集方針やラフカットメモを蓄積する
```

### structure/_template.md

```md
# structure-title

## opening

## middle

## ending

## pacing note
```

### cut-notes/_template.md

```md
# cut-note-title

## current issue

## proposed cut

## expected effect
```

---

## sound

### 役割

* BGM方針
* 効果音設計
* ナレーション検討
* 音響演出整理

### CLAUDE.md テンプレート

```md
# sound

## 役割

- 音楽、効果音、ナレーションなど音の演出を整理する
- シーンごとの音響意図を明文化する
```

### music/_template.md

```md
# music-brief-title

## scene

## mood

## tempo

## instrumentation
```

### sfx/_template.md

```md
# sfx-note-title

## scene

## effect

## purpose

## timing
```

---

## art

### 役割

* 世界観設定
* ロケーション整理
* 衣装・小道具メモ
* ビジュアルアセット管理

### CLAUDE.md テンプレート

```md
# art

## 役割

- 世界観や美術要素を整理する
- ロケーション、衣装、小道具、ビジュアル設定を蓄積する
- 他部門が参照しやすい形でアセット情報を残す
```

### worldbuilding/_template.md

```md
# worldbuilding-title

## setting

## rules

## visual motifs

## references
```

### assets/_template.md

```md
# asset-title

## 種別

## 用途

## 状態

## 関連シーン
```

---

## distribution

### 役割

* タイトル案
* 紹介文作成
* 予告編方針
* 公開・告知計画

### CLAUDE.md テンプレート

```md
# distribution

## 役割

- 公開に向けたタイトル、紹介文、予告、告知方針を整理する
- 作品を外部へ届けるための情報設計を担当する
```

### title/_template.md

```md
# title-ideas

## 候補

## 意図

## 印象
```

### promo/_template.md

```md
# promo-plan-title

## target

## key message

## teaser idea

## release plan
```
