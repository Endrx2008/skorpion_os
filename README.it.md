<div align="center">

# 🦂 Skorpion OS

**Una distribuzione Linux leggera con un'IA locale integrata — il tuo maggiordomo, non il tuo padrone.**

[Sito](https://skossite.pages.dev) · [Download](https://sourceforge.net/projects/skos/files/) · [Wiki PN LUG](https://wiki.pnlug.it/index.php?title=Sperimentare_con_Skorpion_OS#Link_al_progetto) · [Instagram](https://www.instagram.com/skorpion.os/) · [Ko-fi](https://ko-fi.com/I3X828AUUL)

*English: [README.md](README.md)*

</div>

---

## Cos'è Skorpion OS?

Skorpion OS è una distribuzione Linux open source con un assistente IA integrato, **SKAI**, basato su
**[Ollama](https://ollama.com)**. L'IA fa parte del sistema, non è un programma a parte: ogni app e
componente SKAI parla con lo stesso modello locale, quindi tutto gira **sul tuo computer** — niente cloud,
niente account, nessun dato inviato a server esterni.

L'IA lavora *con* te, non *al posto tuo*. Si occupa del lavoro d'ufficio e dell'uso quotidiano del computer
per lasciarti più tempo per ciò che conta — arte, cultura, le tue idee. Skorpion OS vuole insegnare a chi
inizia e dare potere agli esperti. E se l'IA non la vuoi, SKAI Manager la spegne.

**Versione attuale: 4.0** · Presente su [DistroWatch](https://distrowatch.com/table.php?distribution=skorpion)

## Filosofia

- 🤵 **L'IA come maggiordomo, non come padrone** — aiuta, non prende il controllo
- 🔒 **La privacy è un diritto** — modelli locali, dati locali
- 🧱 **Tante basi, nessun limite** — basi e desktop diversi, scegli tu
- 🪶 **Leggero e libero** — un sistema che rispetta il tuo hardware e la tua libertà
- 💚 **Open source per scelta**

Skorpion OS è contro l'IA che rende pigri e contro l'IA che sostituisce gli artisti.

## Edizioni

| Edizione | Base | Desktop | Dimensione | Ideale per |
|---|---|---|---|---|
| **Cinnamon** | Debian | Cinnamon | 3,6 GB | Desktop completo — consigliata per la prima installazione |
| **Lite** | Debian | i3 | 3,3 GB | Hardware datato o una base minima |
| **Mantis** | Arch | Hyprland | 2,9 GB | Rolling release con un compositor a tiling |

Ogni edizione parte con la procedura guidata di SKAI, che installa Ollama e il modello che scegli, e
include tutta la suite SKAI: SKAI Manager (Alt + F9), sk_files e i componenti per Firefox,
Thunderbird e LibreOffice. Lite e Mantis aggiungono il launcher Skorpion (Alt + F1) con la multicalcolatrice
e la guida (Alt + F3); Cinnamon tiene il suo menu. La sessione
live parte senza password. ISO e checksum sono su [SourceForge](https://sourceforge.net/projects/skos/files/).

## Requisiti minimi

| Risorsa | Requisito |
|---|---|
| **CPU** | 4+ core, x86_64, Intel/AMD con AVX2 |
| **RAM** | 8 GB (16 GB per il modello consigliato, qwen2.5:14b) |
| **GPU** | 4 GB di VRAM — consigliata NVIDIA con CUDA 11+ |
| **Spazio** | 20 GB+ |
| **Internet** | serve al primo avvio per scaricare Ollama e il modello |

Sui computer meno potenti si possono scegliere nella procedura guidata modelli più piccoli (fino a
qwen2.5:3b). La ricerca web (DuckDuckGo) serve solo a cercare informazioni — mai a elaborare i tuoi dati.

## L'ecosistema SKAI

| Repository | Cos'è | Come si ottiene |
|---|---|---|
| [skai_manager](https://github.com/Endrx2008/skai_manager) | procedura guidata di SKAI e SKAI Manager: modelli, acceso/spento, PC remoto | nella ISO |
| [launcher](https://github.com/Endrx2008/launcher) | launcher Skorpion con chat SKAI, multicalcolatrice, guida (Lite, Mantis) | nella ISO |
| [sk_files](https://github.com/Endrx2008/sk_files) | assistente per i file da terminale, a parole | nella ISO |
| [sk_notes](https://github.com/Endrx2008/sk_notes) | note in Markdown per PC e Android, e SKAI_ Memory, la memoria condivisa da tutte le app SKAI | [release](https://github.com/Endrx2008/sk_notes/releases/latest): .deb, pacchetto Arch, APK |
| [sk_office](https://github.com/Endrx2008/sk_office) | SKAI per LibreOffice — Writer, Calc e Math | [release](https://github.com/Endrx2008/sk_office/releases/latest): .oxt |
| [sk_mail](https://github.com/Endrx2008/sk_mail) | SKAI per Thunderbird — posta e calendario | [release](https://github.com/Endrx2008/sk_mail/releases/latest): .xpi |
| [skaifox](https://github.com/Endrx2008/skaifox) | SKAI per Firefox — cerca, apre e legge pagine | [release](https://github.com/Endrx2008/skaifox/releases/latest): .xpi |

Anche in copia su [GitLab](https://gitlab.com/Endrx2008).

## Questo repository

Materiale generale del progetto, non il codice delle app (ogni app ha il suo repository, vedi sopra).

| Percorso | Cos'è |
|---|---|
| `system-images/skorpion_logo/` | il logo di Skorpion OS: `skorpion_logo.svg`, `skorpion_logo_white.svg`, con il nome (`skorpion_logo_name.svg`) e l'icona del menu (`menu.png`) |
| `system-images/wallpaper4.png`, `wallpaper4-1.png` | sfondi della versione attuale |
| `ventoy_theme/ventoy.7z` | il tema del menu di avvio per una chiavetta [Ventoy](https://www.ventoy.net): estrailo nella radice della prima partizione della chiavetta (aggiunge `ventoy/ventoy.json` e `ventoy/ventoy-pop/`, 1920×1080) |

**Licenza:** le immagini e il tema Ventoy di questo repository sono rilasciati sotto GPL-3.0-or-later (vedi
[LICENSE](LICENSE)). Skorpion OS è un insieme di molti programmi: ognuno mantiene la propria licenza, e le
app SKAI sono GPL-3.0-or-later nei loro repository.

## Roadmap

**✅ Fatto**
- ISO Cinnamon, Lite e Mantis
- Procedura guidata di SKAI e SKAI Manager · launcher · sk_files · skaifox · sk_office · sk_mail
- SKAI_ Memory, la memoria condivisa dalle app · sk_notes 0.5.0 per PC e Android

**🚧 In corso**
- **flowforge** — app store per creare le tue app con il vibe coding
- **sk_images** — ricerca di immagini con l'IA

**🗓️ In programma**
- **skai-finetune** — fine-tuning del modello per un'integrazione più precisa

## Contribuire

Skorpion OS è sviluppato da un solo manutentore — **cerchiamo collaboratori!** L'aiuto serve soprattutto per:

- i moduli SKAI e la memoria condivisa tra le app
- plugin per programmi esistenti
- backend Python e integrazione con il desktop
- la creazione delle ISO
- l'estensione per il browser

Apri una issue, manda una pull request, o vieni agli incontri del [PN LUG](https://pnlug.it) a Pordenone,
ogni martedì sera. Puoi anche sostenere il progetto su [Ko-fi](https://ko-fi.com/I3X828AUUL) 💚

---

<div align="center">

Fatto con 🦂 da **Enrico Miot (EndrX)** — fondatore e manutentore

</div>
