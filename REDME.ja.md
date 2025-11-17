# **sjtmp-vault-template**

個人向けの Zettelkasten（ツェッテルカステン）風ワークフロー  
**Seed → Journal → Theme → Meta → Publish（SJTMP）**  
を Obsidian 上で再現可能にするためのテンプレートです。

このリポジトリには以下が含まれます：

- ミニマルなフォルダ構成  
- 日本語／英語のノートテンプレート  
- 任意で使える AI アシスト（Smart Composer + Claude API）  

これらにより、「外部脳」として Obsidian を複数端末で安定して運用できます。

---

## **ディレクトリ構造**

```text
00_Seed/       — 生メモ・ひらめきの一時置き場
01_Journal/    — 観察・記録・内省
02_Theme/
  ├ Private/   — 個人的な反復テーマ
  └ Public/    — 外部化できる一般化されたテーマ
03_Meta/       — 概念構造・抽象モデル
04_Publish/    — 公開用ドラフト
templates/     
  ├ en-us/     — 英語版テンプレート
  ├ ja-jp/     — 日本語版テンプレート
  └ prompts/   — Smart Composer 用プロンプト定義（JSON + MD）
```

この構造は SJTMP のフロー：

- **Seed → Journal → Theme → Meta → Publish**

にそのまま対応しています。

---

## **推奨 Obsidian セットアップ（任意だが強力）**

この Vault は次の 3 つの Obsidian プラグインに最適化されています：

- **Templater**  
- **Smart Composer**（Claude API / OpenAI）
- **Obsidian Git**

複数端末で同じ環境を再現したい場合は、以下の手順でセットアップしてください。

### **1. リポジトリをクローン**

```sh
git clone https://github.com/your/repo.git
```

### **2. Obsidian で Vault として開く**

### **3. 必要なプラグインをインストール**

1. **Templater**  
2. **Smart Composer**  
3. **Obsidian Git**

### **4. Smart Composer のプロンプトを再インポート**

Smart Composer は **設定を自動同期しません**。

この Vault 内の以下のパスに、  
すべてのプロンプト定義（JSON + Markdown）が入っています：

```path
templates/prompts/smart-composer/
```

とくに重要なのが：

```path
_sjtmp-prompts.md   — System Prompt + 全 SJTMP プロンプトの決定版
```

Smart Composer → Prompt Templates → “New Template” から  
各プロンプトの本文をコピペして設定してください。

### **5. Seed を取り始める**

- スマートフォン：`00_Seed/` に直接メモ  
- デスクトップ：Smart Composer で昇格  
  （Seed → Journal → Theme → Meta → Publish）

---

## **複数端末セットアップのチェックリスト**

新しい端末で再構築するときは：

1. リポジトリを clone  
2. Obsidian をインストール  
3. Templater / Smart Composer / Obsidian Git を入れる  
4. `_sjtmp-prompts.md` から Prompt を再設定  
5. Obsidian Git で pull/push  

これにより、ローカル DB やプラグイン本体を同期せずとも  
**100％ 同じ環境を再現できます。**

---

## **使い方**

1. `00_Seed/` に素早くメモを書き留める  
2. 成熟したら順次 SJTMP の階層へ昇格  
3. 必要に応じて Smart Composer を利用  
4. `04_Publish/` で公開用ドラフトへ仕上げる  

---

## **ライセンス**

MIT（または任意のライセンスを使用してください）
