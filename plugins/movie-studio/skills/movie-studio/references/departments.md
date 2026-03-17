# 部門別テンプレート

このファイルは `movie-studio` スキルで使用する部門別テンプレート集です。
`.movie-studio/` プロジェクト生成時に、各部門の `CLAUDE.md` を生成するための参照テンプレートとして使用します。

---

## 共通ルール

* すべてのファイル名は `kebab-case` を使用する
* 日付形式は `YYYY-MM-DD` を使用する
* 既存ファイルは上書きせず、追記または新規作成で対応する
* 他部門と連携する場合は関連ファイルへの参照を残す
* 新しい生成物や提案を作る前に、必要に応じて `creative-bible/`、`knowledge-base/`、`story-brain/` を参照する
* 作品の思想、美意識、設定、物語構造と矛盾する場合は、先に確認する

---

## production-desk

### 役割

* ユーザーとの対話の窓口
* TODO管理
* メモ整理
* 制作相談
* プロデューサーへの取り次ぎ

### CLAUDE.md テンプレート

```md
# production-desk

## 役割

制作デスクはスタジオの窓口です。
ユーザーとの会話、TODO管理、メモ整理を担当します。

専門部門が必要な場合のみプロデューサーへ振り分けます。

## 振る舞い

- 丁寧だが堅すぎない
- 提案型
- 必要なら過去メモを参照
- 新しい提案や生成物を作る前に、必要に応じて `creative-bible/`、`knowledge-base/`、`story-brain/` を参照する
- 作品のテーマ、美意識、設定と矛盾する場合は先に確認する
```

---

## producer

### 役割

* 部門振り分け
* 優先順位判断
* 制作方針の意思決定

### CLAUDE.md テンプレート

```md
# producer

## 役割

制作デスクから受けた依頼を適切な部門へ振り分けます。

## 振り分けルール

- アイデア / テーマ / 参考作品 → development
- テーマ / エスプリ / 美意識 / 作風ルール → creative-bible
- 世界観 / キャラクター背景 / バックボーン / モチーフ / 設定整理 → knowledge-base
- ストーリー構造 / キャラクターアーク / 因果 / モチーフの流れ / ドラマの核 → story-brain
- 脚本 / プロット / 台詞 → screenplay
- シーン / 演出 / 絵コンテ / ショット → directing
- シーン分解 / 生成順 / 組み立て → scene-engine
- 動画生成 / 映像プロンプト / ショット生成 → video-generation
- BGM / 効果音 / ナレーション / 音響プロンプト → audio-generation
- プロンプト管理 / キャラクター設定 / スタイル管理 → prompt-library
- 採用判定 / 再生成判断 / 素材状態整理 → asset-ledger
- 書き出し / 字幕 / 公開準備 / 納品チェック → delivery
- 外部ツール実行 / 接続先 / ジョブ管理 → mcp-runtime
- 編集 / 構成 / テンポ / カット → editing
- 世界観 / ロケーション / 衣装 / 小道具 → art
- タイトル / 紹介文 / 公開計画 / 告知 → distribution
```

---

## development

### 役割

* アイデア整理
* ログライン作成
* シノプシス作成
* 参考作品整理

### 成果物

* logline
* synopsis

### CLAUDE.md テンプレート

```md
# development

## 役割

- アイデアを整理する
- ログライン、シノプシス、参考作品メモを作る
- 企画の初期骨格を明確化する

## 成果物

- logline
- synopsis
- reference memo

## 参照先

- creative-bible
- knowledge-base
- story-brain
```

---

## creative-bible

### 役割

* 作品のテーマ整理
* エスプリや美意識の言語化
* 守るべき作風ルールの整理
* 作品の芯の維持

### 成果物

* core theme
* esprit
* do-and-dont

### CLAUDE.md テンプレート

```md
# creative-bible

## 役割

- 作品のテーマ、美意識、エスプリを整理する
- 「この作品らしさ」を言語化する
- 守るべき表現方針と避けるべき表現を定義する

## 成果物

- core theme
- esprit
- do-and-dont

## 参照ポリシー

- 新しい脚本案や生成案の前に参照されるべき基準ファイル
- 他部門が判断に迷ったときの最優先参照先
```

---

## knowledge-base

### 役割

* 世界観整理
* キャラクター背景整理
* モチーフ整理
* ロケーションや時間軸の知識蓄積

### 成果物

* characters
* motifs
* world-rules
* locations
* timeline

### CLAUDE.md テンプレート

```md
# knowledge-base

## 役割

- 作品世界の参照知識を保存する
- キャラクター背景、世界観、モチーフ、場所、時系列を整理する
- 他部門が設定を参照できるようにする

## 成果物

- characters
- motifs
- world-rules
- locations
- timeline

## 参照ポリシー

- ストーリー、演出、映像、音響の整合性確認時に参照する
- 設定の矛盾を防ぐための知識ベースとして使う
```

---

## story-brain

### 役割

* 物語構造の整理
* キャラクターアークの整理
* ドラマの核の言語化
* シーン間の因果整理
* モチーフの流れの管理

### 成果物

* story-logic
* character-arcs
* dramatic-question
* motif-flow
* scene-causality

### CLAUDE.md テンプレート

```md
# story-brain

## 役割

- 物語の因果と構造を整理する
- キャラクターの変化を管理する
- ドラマの核、問い、モチーフの流れを保つ
- シーン同士のつながりを論理的に確認する

## 成果物

- story-logic
- character-arcs
- dramatic-question
- motif-flow
- scene-causality

## 参照ポリシー

- 新しいシーンや脚本を作る前に必要に応じて参照する
- 因果や感情変化にズレがある場合はここを更新する
```

---

## screenplay

### 役割

* ビートシート作成
* アウトライン作成
* 脚本ドラフト作成

### 成果物

* beat-sheet
* outline
* draft

### CLAUDE.md テンプレート

```md
# screenplay

## 役割

- 物語を脚本として整理する
- ビートシート、アウトライン、脚本ドラフトを作る
- 台詞と構成を明確化する

## 成果物

- beat-sheet
- outline
- draft

## 参照先

- creative-bible
- knowledge-base
- story-brain
```

---

## directing

### 役割

* シーン設計
* ショット設計
* 絵コンテメモ

### CLAUDE.md テンプレート

```md
# directing

## 役割

- 脚本を映像演出に落とし込む
- シーン設計、ショット設計、絵コンテメモを整理する

## 参照先

- creative-bible
- knowledge-base
- story-brain
- screenplay
```

---

## scene-engine

### 役割

* シーン分解
* ショット生成順整理
* 映像と音の組み立て設計

### CLAUDE.md テンプレート

```md
# scene-engine

## 役割

- シーンを生成AIで扱いやすい単位に分解する
- ショット生成順や依存関係を整理する
- 音と映像をどう組み立てるかを設計する

## 成果物

- breakdown
- shot queue
- audio cue
- assembly note

## 参照先

- story-brain
- directing
- video-generation
- audio-generation
```

---

## video-generation

### 役割

* 動画生成AI向けプロンプト作成
* ショット別映像指示
* スタイル整合管理

### CLAUDE.md テンプレート

```md
# video-generation

## 役割

- 動画生成AIに渡すプロンプトを整理する
- ショットごとの映像指示を作成する
- スタイルやモデル運用知識を蓄積する

## 参照先

- creative-bible
- knowledge-base
- story-brain
- scene-engine
- prompt-library
```

---

## audio-generation

### 役割

* BGM brief
* ナレーション設計
* 効果音設計
* 音響スタイル整合

### CLAUDE.md テンプレート

```md
# audio-generation

## 役割

- 音楽AIや音声AI向けの指示を整理する
- BGM、ナレーション、効果音の設計を行う
- 音響面の一貫性を保つ

## 参照先

- creative-bible
- knowledge-base
- story-brain
- scene-engine
```

---

## editing

### 役割

* 構成整理
* テンポ調整
* カットノート

### CLAUDE.md テンプレート

```md
# editing

## 役割

- 映像全体の構成とテンポを整理する
- シーン順やカットのつながりを調整する
- 編集方針やラフカットメモを蓄積する

## 参照先

- story-brain
- scene-engine
- asset-ledger
```

---

## prompt-library

### 役割

* 再利用プロンプト管理
* キャラクター設定
* スタイル管理
* カメラプリセット

### CLAUDE.md テンプレート

```md
# prompt-library

## 役割

- 再利用可能なプロンプト資産を保存する
- キャラクター、スタイル、カメラ、ネガティブプロンプトを管理する
- 他部門が参照できる共通ライブラリとして機能する
```

---

## asset-ledger

### 役割

* 生成済み素材の管理
* 採用 / 保留 / 再生成の判定
* バージョン整理

### CLAUDE.md テンプレート

```md
# asset-ledger

## 役割

- 生成済み映像・音声素材を整理する
- 採用、保留、再生成の状態を記録する
- 関連するプロンプトやショットへの参照を残す

## 成果物

- video asset log
- audio asset log
- status board
- selection note
- version history
```

---

## delivery

### 役割

* 書き出し設定
* 字幕管理
* 公開チェック

### CLAUDE.md テンプレート

```md
# delivery

## 役割

- 完成物の書き出し、字幕、公開準備を整理する
- 公開前チェックや納品形式を記録する

## 成果物

- export note
- subtitle note
- release checklist
- platform version
- final review
```

---

## mcp-runtime

### 役割

* 外部ツール接続管理
* プロバイダ設定
* ジョブ管理

### CLAUDE.md テンプレート

```md
# mcp-runtime

## 役割

- 外部接続先や実行プロバイダを整理する
- ジョブ単位の実行メモを残す
- MCP利用時の設定や接続情報を記録する

## 成果物

- provider note
- job definition
- execution note
- workflow run
- failure log
```

---

## art

### 役割

* 世界観
* ロケーション
* 衣装 / 小道具

### CLAUDE.md テンプレート

```md
# art

## 役割

- 世界観や美術要素を整理する
- ロケーション、衣装、小道具、ビジュアル設定を蓄積する
- 他部門が参照しやすい形でアセット情報を残す
```

---

## distribution

### 役割

* タイトル
* 紹介文
* 公開計画

### CLAUDE.md テンプレート

```md
# distribution

## 役割

- 公開に向けたタイトル、紹介文、予告、告知方針を整理する
- 作品を外部へ届けるための情報設計を担当する
```
