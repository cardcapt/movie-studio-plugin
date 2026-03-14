# development/synopsis/_template.md

```md
# synopsis-title

- created_at: YYYY-MM-DD
- status: draft
- owner: development

## logline reference

<!-- 関連するログラインへの参照 -->

## 概要

<!-- 作品全体の短い要約 -->

## 起

<!-- 物語の導入。主人公、状況、発端 -->

## 承

<!-- 展開。対立、障害、関係の変化 -->

## 転

<!-- 大きな転換点、危機、真相の露出 -->

## 結

<!-- クライマックスと結末 -->

## テーマ

<!-- この物語で描きたい核 -->

## 感情の流れ

<!-- 主人公や観客にどう感じてほしいか -->

## notes

<!-- 改善点、検討メモ、参考作品メモ -->
```

## 配置先

```text
plugins/movie-studio/skills/movie-studio/references/templates/development/synopsis/_template.md
```

## 補足

* `logline` から `beat-sheet` へつなぐ中間成果物として使う
* 長さは 300〜800 字程度の要約を想定
* 必要なら `起承転結` ではなく `3幕構成` に置き換えてもよい

---

# screenplay/drafts/_template.md

```md
# screenplay-draft-title

- created_at: YYYY-MM-DD
- status: draft
- owner: screenplay
- version: v1

## logline reference

<!-- 対応するログライン -->

## synopsis reference

<!-- 対応するシノプシス -->

---

## FADE IN

<!-- 脚本開始 -->

### SCENE 1

INT./EXT. LOCATION - TIME

Action:

<!-- シーンの状況説明 -->

Dialogue:

CHARACTER NAME

セリフ

---

### SCENE 2

INT./EXT. LOCATION - TIME

Action:

<!-- シーンの状況説明 -->

Dialogue:

CHARACTER NAME

セリフ

---

## notes

<!-- 修正メモ、演出意図、変更履歴など -->
```

## 配置先

```text
plugins/movie-studio/skills/movie-studio/references/templates/screenplay/drafts/_template.md
```

## 補足

* beat-sheet から発展させた脚本ドラフト
* version フィールドで改稿管理（v1, v2, v3...）
* 必要なら `scene` 単位で別ファイルに分割してもよい
