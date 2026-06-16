<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/keepvidya-logo-dark.svg" />
  <img alt="Keepvidya" src="assets/keepvidya-logo-light.svg" width="360" />
</picture>

# Own your intelligence.

**Private AI that runs on your machine — and actually makes you smarter.**

![Local-first](https://img.shields.io/badge/local--first-1B2A33?style=flat-square)
![Private by default](https://img.shields.io/badge/private_by_default-C0703C?style=flat-square)
![Runs offline](https://img.shields.io/badge/runs_offline-1B2A33?style=flat-square)
![Open source](https://img.shields.io/badge/open_source-MIT-C0703C?style=flat-square)

</div>

---

Most AI reads your private documents on **someone else's computer**, charges you to re-read them
**every single time**, and forgets all of it the second you close the tab. You walk away having learned
nothing and kept nothing.

Keepvidya is the opposite — in **two pieces you can use today**, both on your own laptop, neither phoning home.

---

## <img src="assets/docnest-logo.svg" alt="DOCNEST" height="30" align="absmiddle" /> First, the engine: DOCNEST

Here's a revenue table the way most RAG tools hand it to an AI:

```
"45.2%  Q3  Europe  38.1%  Q2  Europe  41.7%  Q3  Asia  29.3%  Q2  Asia"
```

Numbers with no meaning. The model is guessing. Now the same table, the way **DOCNEST** hands it over:

```json
{ "section": "§4.2 Revenue by Region",
  "table": { "headers": ["Region", "Q2", "Q3"],
             "rows": [["Europe", "38.1%", "45.2%"], ["Asia", "29.3%", "41.7%"]] } }
```

Same table. One of them the model can actually reason about. DOCNEST reads a document's **structure
before its content** — every heading a navigable section, every table kept intact — and writes it all
into a portable `.udf` file.

Do that across a whole document and something strange happens: **most factual questions stop needing the
LLM at all.** DOCNEST answers them straight from the structure it already built —

> **80% of factual queries. 100% accuracy. ~92% fewer tokens** than ordinary RAG.

The bill for *"what was Q3 revenue?"* becomes **zero**. The LLM only shows up when you actually need it
to think. Oh — and any AI agent can plug into it over MCP.

[**DOCNEST →**](https://github.com/tailorgunjan93/docnest) · [`pip install docnest-ai`](https://pypi.org/project/docnest-ai/) · [How the parser works](https://coderlegion.com/18673/i-built-a-pdf-parser-that-actually-preserves-table-structure-for-rag-heres-why-it-matters)

---

## <img src="assets/knovex-icon.png" alt="Knovex" height="30" align="absmiddle" /> Then, the app: Knovex

Cloud notebooks let you *chat* with your documents. **Knovex makes you learn them.**

Drop in a PDF and it'll quiz you, build flashcards that resurface on a spaced-repetition schedule, or
turn the topic into an **animated lesson that draws itself one idea at a time** — the way a good teacher
uses a whiteboard. There are XP, levels, and streaks, because finishing things is more fun than starting them.

It's a real desktop app — **Windows, macOS, Linux, auto-updating** — with cited answers, summaries, and
optional web search. Bring your own AI key, or run it **fully offline**. Your files never leave the
machine unless you flip web search on yourself.

And when you're done, you keep a **`.udf`** — a single portable file with your document's knowledge baked
in. Email it, back it up, carry it to a new laptop. It's *yours*, in an [open format](https://github.com/tailorgunjan93/udf-spec) no
vendor controls.

[**⬇ Download Knovex →**](https://tailorgunjan93.github.io/knovex/) · [Repo](https://github.com/tailorgunjan93/knovex) · [The build story](https://coderlegion.com/19280/i-built-a-local-first-ai-desktop-knowledge-base-heres-what-i-learned)

---

## Why this is the whole point

| Cloud AI | Keepvidya |
|---|---|
| Your documents leave your machine | They stay on your hardware |
| Re-embeds — and re-bills — every query | Embed once, query for free |
| You chat, then forget | You **learn it**, and keep a `.udf` |
| Vendor lock-in | Open format, swappable models, MIT |

The name says it: **Keep** + **Vidya** (Sanskrit for *knowledge*) — *keep your knowledge.* The defensible
idea was never "AI." It's **local-first**: the private alternative to the cloud, where your data is yours
by default, not by permission.

---

## Also shipping, and what's next

- **🟣 DocNest .NET** — the same engine, native for **.NET 8** on NuGet. Its `.udf` files are
  **byte-compatible** with the Python ones (proven by interop tests, not promises). For the enterprise and
  the regulated shops that live in C#. → [Repo](https://github.com/tailorgunjan93/docnest-net) · [Why it exists](https://coderlegion.com/20665/your-net-rag-stack-hides-a-python-sidecar-i-built-the-engine-that-removes-it)
- **🔜 Keepvidya Flows** — agents that act on your knowledge. *On the roadmap.*
- **🔜 Keepvidya Core** — small models running fully on-device. *On the roadmap.*

We lead with what's live and mark the future as the future. Under-claim, over-deliver.

---

> **A quick note — “Gunjan” is becoming Keepvidya.** These products were built by
> **Gunjan Tailor** ([@tailorgunjan93](https://github.com/tailorgunjan93)) and are moving under the
> **Keepvidya** organization. Repos still live under `tailorgunjan93/*` during the migration — every link
> above points to its real, working home. More deep-dives on
> [CoderLegion](https://coderlegion.com/user/Gunjan+Tailor) (561 points, 20 badges) and
> [DEV](https://dev.to/gunjantailor/i-built-a-local-first-ai-desktop-knowledge-base-heres-what-i-learned-3o4a).

---

<div align="center">

**Two products live. Nothing leaves your machine.**

[**Download Knovex**](https://tailorgunjan93.github.io/knovex/) · [**Star DOCNEST**](https://github.com/tailorgunjan93/docnest) · [**Read the `.udf` spec**](https://github.com/tailorgunjan93/udf-spec)

### Own your intelligence.

Questions, partnerships, or just hello → **[founder@keepvidya.com](mailto:founder@keepvidya.com)**

<sub>DOCNEST & DocNest .NET — MIT · UDF — CC BY 4.0 · Ink `#1B2A33` + Copper `#C0703C`</sub>

</div>
