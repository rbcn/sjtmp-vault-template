# sjtmp-vault-template

A template for a personalized Zettelkasten workflow:  
**Seed → Journal → Theme → Meta → Publish (SJTMP)**

This repository provides a minimal folder structure, note templates,  
and optional AI-assisted tooling for structuring your thinking with Obsidian.

---

## Directory Structure

```text
00_Seed/       — raw notes / quick capture
01_Journal/    — observations / reflections
02_Theme/
  ├ Private/   — personal recurring themes
  └ Public/    — generalizable themes
03_Meta/       — conceptual models / structure
04_Publish/    — external outputs (drafts)
templates/     — note templates (SJTMP + Smart Composer prompts)
````

> This structure mirrors the intended knowledge flow:
> **Seed → Journal → Theme → Meta → Publish**

---

## Recommended Obsidian Setup (Optional but Powerful)

This vault is optimized for:

* **Templater**
* **Smart Composer** (Claude/OpenAI)
* **Obsidian Git**

If you want full reproducibility across multiple devices:

### 1. Clone the repository locally

```sh
git clone https://github.com/your/repo.git
```

### 2. Open the folder as a Vault in Obsidian

### 3. Install required plugins

1. *Templater*
2. *Smart Composer*
3. *Obsidian Git*

### 4. Configure Smart Composer (one-time per device)

Smart Composer does not sync settings automatically.
Use the prompts stored in:

```
templates/_prompts/obsidian-smart_composer/
```

especially:

```
_sjtmp-prompts.md   — canonical source of all SJTMP prompt templates
```

For each prompt:

* Open Smart Composer → Prompt Templates → New Template
* Copy/paste content from the markdown file
* Give it the same name (recommended)

### 5. Start capturing Seeds

* On mobile: create a new note in `00_Seed/`
* On desktop: promote using Smart Composer (Seed → Journal → Theme → Meta → Publish)

---

## Multi-Device Notes

To set up a new machine:

1. Clone the repo
2. Install Obsidian
3. Install the three plugins
4. Re-import Smart Composer prompts from `_sjtmp-prompts.md`
5. Pull/push via Obsidian Git

This ensures perfect reproducibility without syncing plugin binaries or local DBs.

---

## Usage

1. Start jotting raw ideas in **`00_Seed/`**
2. Promote them naturally through the SJTMP layers
3. Use Smart Composer for optional structured transformation
4. Publish drafts from **`04_Publish/`**

---

## License

MIT (or your preferred license)
