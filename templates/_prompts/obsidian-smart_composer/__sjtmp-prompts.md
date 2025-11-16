# SJTMP Prompt Templates for Obsidian Smart Composer Plugin

外部脳SJTMPフロー（Seed → Journal → Theme → Meta → Publish）で利用する、
Smart Composer プロンプトの保存版。

各端末で Smart Composer をセットアップする際は、
GUI から “New Template” を作成し、以下のプロンプト本文を貼り付けてください。

---

## 🟢 1. Extract Seeds  

**name:** `extract-seeds`

```prompt
この文章から、後で育てられるSeed候補を抽出してください。
短く、断片的で、メモ的で構いません。
なるべく多くの可能性を保存する方向で、箇条書きにしてください。
````

[Setting JSON](_extract-seeds.json)

---

## 🟣 2. Promote Seed → Journal

**name:** `promote-s2j`

```prompt
このSeedをもとに、自然で流れるようなJournalに昇格させてください。
思考の粗さは保持しつつ、最小限の文脈を補い、過度に整えないでください。
ユーザーの文体・温度・リズムは絶対に壊さず、
観察・気づき・内的モノローグの形でまとめてください。
```

[Setting JSON](_promote-s2j.json)

---

## 🟡 3. Promote Journal → Theme

**name:** `prompt-j2t`

```prompt
このJournalから、くり返し現れているパターン、意味軸、傾向を抽出し、
1つのThemeノートとしてまとめてください。
抽象化しすぎず、具体的な文脈を残しながら、
「そのテーマが何を語っているか」を整理してください。
ユーザーの声を保持してください。
```

[Setting JSON](_promote-j2t.json)

---

## 🔵 4. Promote Theme → Meta

**name:** `prompt-t2m`

```prompt
このThemeをもとに、背後にある構造・因果・概念・メカニズムを取り出し、
Metaノートとして整理してください。
学術化しすぎず、ユーザーの語りの温度を維持しつつ、
思考の骨格となる抽象モデルを生成してください。
```

[Setting JSON](_promote-t2m.json)

---

## 🟠 5. Generate Publish Draft from Meta

**name:** `gen-draft-m2p`

```prompt
このMetaノートの内容をもとに、外部公開向けのPublish Draftを生成してください。
文章の流れ、読みやすさ、構造化を強化しつつ、
ユーザー固有の文体・比喩・語りを保持してください。
導入・展開・結論の流れを自然に整え、Hashnodeで読まれることを想定してください。
```

[Setting JSON](_gen-draft-m2p.json)

---

## ⚪ 6. Generic Polish (Keep Voice)

**name:** `polish-keep-voice`

```prompt
この文章を読みやすく整えてください。
ただし、ユーザーの文体・語尾・間合い・比喩・世界観を絶対に壊さないでください。
情報の削除や追加は行わず、構造と文章の滑らかさのみを改善してください。
```

[Setting JSON](_polish-keep-voice.json)

---
