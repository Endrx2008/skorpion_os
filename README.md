<div align="center">

# 🦂 Skorpion OS

**A lightweight Linux distribution with a local AI built in — your butler, not your master.**

[Website](https://skossite.pages.dev) · [Download](https://sourceforge.net/projects/skos/files/sk_os.iso/download) · [PN LUG Wiki](https://wiki.pnlug.it/index.php?title=Sperimentare_con_Skorpion_OS#Link_al_progetto) · [Instagram](https://www.instagram.com/skorpion.os/) · [Ko-fi](https://ko-fi.com/I3X828AUUL)

</div>

---

## What is Skorpion OS?

Skorpion OS is an open source Linux distribution that ships with an integrated AI assistant, **SKAI**, powered by **[Ollama](https://ollama.com)**. AI is not a separate program here: it is part of the system. Every component talks to a single local model, so everything runs **on your machine** — no cloud, no accounts, no data sent to external servers.

The AI works *alongside* you, not *instead of* you. It simplifies office work and everyday computing so you have more time for what matters — art, culture, your own ideas. Skorpion OS aims to teach beginners and give power to experts. And if you don't want the AI, you can remove it with a single click.

**Current version: 4.0** · Listed on [DistroWatch](https://distrowatch.com/table.php?distribution=skorpion) · Licensed under **GPLv3**

## Philosophy

- 🤵 **AI as a butler, not a master** — it assists, it doesn't take over
- 🔒 **Privacy is a right** — local models, local data
- 🧱 **Many foundations, no limits** — different bases and desktops, your choice
- 🪶 **Lightweight and free** — a system that respects your hardware and your freedom
- 💚 **Open source by choice**

Skorpion OS is against AI that makes people lazy and against AI that replaces artists.

## Editions

| Edition | Base | Desktop | Size | Best for |
|---|---|---|---|---|
| **Cinnamon** | Debian | Cinnamon | 3.6 GB | Full desktop — recommended for your first install |
| **Lite** | Debian | i3 | 3.3 GB | Older hardware or a minimal base |
| **Mantis** | Arch | Hyprland | 2.9 GB | Rolling release with a tiling compositor |

All editions include the full AI suite. The live session boots without a password.
ISOs and checksums are on [SourceForge](https://sourceforge.net/projects/skos/files/).

## Minimum requirements

| Resource | Requisite |
|---|---|
| **CPU** | 4+ cores, x86_64, Intel/AMD with AVX2 |
| **RAM** | 8 GB (16 GB for the recommended model, qwen2.5:14b) |
| **GPU** | 4 GB VRAM — NVIDIA with CUDA 11+ recommended |
| **Storage** | 20 GB+ |
| **Internet** | Needed at first boot to download Ollama and the model |

Smaller models can be chosen at setup for less powerful machines.

Web search (via DuckDuckGo) is used only to look things up — never to process your data.

## Roadmap

**✅ Done**
- Debian + i3 ISO (Lite) · Debian + Cinnamon ISO (Cinnamon) · Arch + Hyprland ISO (Mantis)
- Skaifox · skai-cli · SKAI Launcher · SKAI Wizard · sk_libre · sk_mail

**🚧 In progress**
- **flowforge** — app store to build your own apps with vibe coding
- **sk_images** — AI-powered image search
- **Shared memory** across apps and **sk_notes**, a notes app

**🗓️ Planned**
- **skai-finetune** — model fine-tuning for a more precise integration

## Contributing

Skorpion OS is currently developed by a single maintainer — **we're looking for collaborators!**
Areas where help is most welcome:

- SKAI module integration and shared memory between apps
- Plugins for existing software
- Python backend and desktop integrations
- ISO packaging
- Browser extension

Open an issue, send a pull request, or come to the [PN LUG](https://pnlug.it) meetings in Pordenone, every Tuesday evening.
You can also support the project on [Ko-fi](https://ko-fi.com/I3X828AUUL) 💚

## 🌐 Media


🌐 [Website](https://skossite.pages.dev)

🔗 [Download folder](https://sourceforge.net/projects/skos/files/sk_os.iso/download)

📸 [Instagram](https://www.instagram.com/skorpion.os/)

📝 [Pnlug Wiki](https://wiki.pnlug.it/index.php?title=Sperimentare_con_Skorpion_OS#Link_al_progetto)


## The SKAI ecosystem

| Repo | Description |
|---|---|
| [skai_manager](https://github.com/Endrx2008/skai_manager) | SKAI Manager — local AI control center and first-boot wizard |
| [sk_notes](https://github.com/Endrx2008/sk_notes) | skai_Notes — notes and .md memory |
| [sk_files](https://github.com/Endrx2008/sk_files) | skai-cli — natural-language terminal file manager |
| [sk_office](https://github.com/Endrx2008/sk_office) | SKAI for LibreOffice — Writer, Calc and Math extensions |
| [sk_mail](https://github.com/Endrx2008/sk_mail) | SKAI for Thunderbird — mail and calendar add-on |
| [skaifox](https://github.com/Endrx2008/skaifox) | SKAI for Firefox — search assisted add-on |
| [launcher](https://github.com/Endrx2008/launcher) | SKAI Launcher for Lite (i3) and Mantis (Hyprland) |


Also mirrored on [GitLab](https://gitlab.com/Endrx2008).

---

<div align="center">

Made with 🦂 by **EndrX** — founder and main maintainer

Thank you for visiting

</div>
