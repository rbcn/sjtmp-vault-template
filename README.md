# **sjtmp-vault-template**

A reproducible Obsidian vault template for a personalized
Zettelkasten-inspired workflow:
**Seed → Journal → Theme → Meta → Publish (SJTMP)**

This repository provides:

* Minimal folder structure
* Note templates (JA/EN)
* Optional AI-assisted tooling (Smart Composer + Claude API)

for running your “external brain” knowledge system across devices.

---

## **Directory Structure**

```text
00_Seed/       — raw notes / quick capture
01_Journal/    — observations / reflections
02_Theme/
  ├ Private/   — personal recurring themes
  └ Public/    — generalizable themes
03_Meta/       — conceptual models / structure
04_Publish/    — external outputs (drafts)
templates/     
  ├ en-us/     — note templates (EN)
  ├ ja-jp/     — note templates (JA)
  └ prompts/   — Smart Composer prompt definitions (JSON + MD)
```

This mirrors the intended knowledge flow:
**Seed → Journal → Theme → Meta → Publish**

---

## **Recommended Obsidian Setup (Optional but Powerful)**

This vault is optimized for three plugins:

* **Templater**
* **Smart Composer** (Claude API / OpenAI)
* **Obsidian Git**

If you want reproducibility across devices:

### **1. Clone the repository**

```sh
git clone https://github.com/your/repo.git
```

### **2. Open the folder as an Obsidian Vault**

### **3. Install required plugins**

1. **Templater**
2. **Smart Composer**
3. **Obsidian Git**

### **4. Re-import Smart Composer prompts**

Smart Composer does *not* sync settings automatically.

Use the canonical config stored in:

```path
templates/prompts/smart-composer/
```

Especially:

```path
_sjtmp-prompts.md   — full system prompt + all SJTMP templates
```

For each prompt:

* Smart Composer → Prompt Templates → “New Template”
* Paste the content
* Use the same `name:` suggested in the file

### **5. Start capturing Seeds**

* On mobile: create notes directly in `00_Seed/`
* On desktop: promote via Smart Composer (Seed → Journal → Theme → Meta → Publish)

---

## **Multi-Device Setup Checklist**

For a new machine:

1. Clone this repo
2. Install Obsidian
3. Install Templater / Smart Composer / Obsidian Git
4. Paste Smart Composer templates from `_sjtmp-prompts.md`
5. Sync via Obsidian Git

This ensures 100% reproducibility without syncing plugin binaries or local DBs.

---

## **Usage**

1. Capture ideas quickly in `00_Seed/`
2. Promote notes naturally through the SJTMP layers
3. Use Smart Composer when helpful
4. Refine Publish drafts in `04_Publish/`

---

## **License**

MIT (or your preferred license)
