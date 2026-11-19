<div align="center">

# 🦂 Skorpion OS

**A lightweight Linux distribution with a local AI built in — your butler, not your master.**

[Website](https://skossite.pages.dev) · [Download](https://sourceforge.net/projects/skos/files/) · [PN LUG Wiki](https://wiki.pnlug.it/index.php?title=Sperimentare_con_Skorpion_OS#Link_al_progetto) · [Instagram](https://www.instagram.com/skorpion.os/) · [Ko-fi](https://ko-fi.com/I3X828AUUL)

*Italiano: [README.it.md](README.it.md)*

</div>

---

## What is Skorpion OS?

Skorpion OS is an open source Linux distribution with a built-in AI assistant, **SKAI**, powered by
**[Ollama](https://ollama.com)**. The AI is part of the system, not a separate program: every SKAI app and
add-on talks to the same local model, so everything runs **on your machine** — no cloud, no account, no data
sent to outside servers.

The AI works *with* you, not *instead of* you. It takes care of office work and everyday computing so you
have more time for what matters — art, culture, your own ideas. Skorpion OS wants to teach beginners and give
power to experts. And if you don't want the AI, SKAI Manager turns it off.

**Current version: 4.0** · Listed on [DistroWatch](https://distrowatch.com/table.php?distribution=skorpion)

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

Every edition starts with the SKAI setup wizard, which installs Ollama and the model you choose, and
includes the whole SKAI suite: SKAI Manager (Alt + F9), sk_files and the add-ons for Firefox,
Thunderbird and LibreOffice. Lite and Mantis add the Skorpion launcher (Alt + F1) with its multicalculator
and the guide (Alt + F3); Cinnamon keeps its own menu. The live
session boots without a password. ISOs and checksums are on [SourceForge](https://sourceforge.net/projects/skos/files/).

## Minimum requirements

| Resource | Requirement |
|---|---|
| **CPU** | 4+ cores, x86_64, Intel/AMD with AVX2 |
| **RAM** | 8 GB (16 GB for the recommended model, qwen2.5:14b) |
| **GPU** | 4 GB VRAM — NVIDIA with CUDA 11+ recommended |
| **Storage** | 20 GB+ |
| **Internet** | needed at first boot to download Ollama and the model |

Smaller models (down to qwen2.5:3b) can be chosen in the wizard for less powerful machines. Web search
(DuckDuckGo) is used only to look things up — never to process your data.

## The SKAI ecosystem

| Repository | What it is | How you get it |
|---|---|---|
| [skai_manager](https://github.com/Endrx2008/skai_manager) | SKAI setup wizard and SKAI Manager: models, on/off, remote PC | in the ISO |
| [launcher](https://github.com/Endrx2008/launcher) | Skorpion launcher with SKAI chat, multicalculator, guide (Lite, Mantis) | in the ISO |
| [sk_files](https://github.com/Endrx2008/sk_files) | terminal file assistant in plain language | in the ISO |
| [sk_notes](https://github.com/Endrx2008/sk_notes) | Markdown notes for PC and Android, and SKAI_ Memory, the memory all SKAI apps share | [release](https://github.com/Endrx2008/sk_notes/releases/latest): .deb, Arch package, APK |
| [sk_office](https://github.com/Endrx2008/sk_office) | SKAI for LibreOffice — Writer, Calc and Math | [release](https://github.com/Endrx2008/sk_office/releases/latest): .oxt |
| [sk_mail](https://github.com/Endrx2008/sk_mail) | SKAI for Thunderbird — mail and calendar | [release](https://github.com/Endrx2008/sk_mail/releases/latest): .xpi |
| [skaifox](https://github.com/Endrx2008/skaifox) | SKAI for Firefox — searches, opens and reads pages | [release](https://github.com/Endrx2008/skaifox/releases/latest): .xpi |

Also mirrored on [GitLab](https://gitlab.com/Endrx2008).

## This repository

General material of the project, not the code of the apps (each app has its own repository, see above).

| Path | What it is |
|---|---|
| `system-images/skorpion_logo/` | the Skorpion OS logo: `skorpion_logo.svg`, `skorpion_logo_white.svg`, with the name (`skorpion_logo_name.svg`) and the menu icon (`menu.png`) |
| `system-images/wallpaper4.png`, `wallpaper4-1.png` | wallpapers of the current release |
| `ventoy_theme/sk_vnt_theme.7z` | **sk_vnt_theme**, the boot-menu theme for a [Ventoy](https://www.ventoy.net) USB stick: extract it at the root of the stick's first partition (it adds `ventoy/ventoy.json` and `ventoy/sk_vnt_theme/`, 1920×1080). Based on ventoy-pop by Diego Duarte, see `CREDITS` in the theme |

**License:** the images and the Ventoy theme of this repository are released under GPL-3.0-or-later (see
[LICENSE](LICENSE)). Skorpion OS itself is a collection of many programs: each keeps its own license, and
the SKAI apps are GPL-3.0-or-later in their own repositories.

## Roadmap

**✅ Done**
- Cinnamon, Lite and Mantis ISOs
- SKAI setup wizard and SKAI Manager · launcher · sk_files · skaifox · sk_office · sk_mail
- SKAI_ Memory, the memory shared by the apps · sk_notes 0.5.0 for PC and Android

**🚧 In progress**
- **flowforge** — app store to build your own apps with vibe coding
- **sk_images** — AI-powered image search

**🗓️ Planned**
- **skai-finetune** — model fine-tuning for a more precise integration

## Contributing

Skorpion OS is developed by a single maintainer — **collaborators are welcome!** Help is most useful for:

- SKAI modules and the shared memory between apps
- plugins for existing software
- Python backend and desktop integration
- ISO packaging
- the browser extension

Open an issue, send a pull request, or come to the [PN LUG](https://pnlug.it) meetings in Pordenone, every
Tuesday evening. You can also support the project on [Ko-fi](https://ko-fi.com/I3X828AUUL) 💚

---

<div align="center">

Made with 🦂 by **Enrico Miot (EndrX)** — founder and maintainer

</div>
