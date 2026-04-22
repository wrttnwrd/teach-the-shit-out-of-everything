# Teach The Shit Out Of Everything

An LLM wiki toolset for teaching the shit out of everything (TTSOOE). It uses Obsidian and Claude Code so an AI assistant can ingest raw source material, maintain an interlinked knowledge base, and draft content briefs grounded in that knowledge base.

This repo includes an example vault and wiki for **Green Slaad Enterprises**. If you want to use it for your own project, delete the contents of the briefs, raw, and wiki folders. **All instructions below assume you've emptied those folders and edited claude.md to suit your requirements.**

More bolded reminders follow.

## Credits

All credit to Andrej Karpathy for his outstanding [LLM Wiki concept](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f), upon which this entire repository is built.

If you want to learn more about teaching the shit out of everything, have a look here:

[https://www.ianlurie.com/digital-marketing/teach-the-shit-out-of-everything/](https://www.ianlurie.com/digital-marketing/teach-the-shit-out-of-everything/)

## Tools

This repository is built on Claude Code and Obsidian. You can implement it using any AI and any text editor capable of viewing Markdown. Or you can read the Markdown in plain text, but why do that to yourself?

- [Claude Code](https://claude.com/claude-code) — the AI assistant that reads `CLAUDE.md` and maintains the wiki.
- [Obsidian](https://obsidian.md) — renders the Markdown and resolves `[[wiki-links]]` between pages.

## Setup

1. **Clone the repository.**

   ```bash
   git clone https://github.com/wrttnwrd/teach-the-shit-out-of-everything.git
   cd teach-the-shit-out-of-everything
   ```

2. **Open the vault in Obsidian.** Choose "Open folder as vault" and select the inner `greenslaadttsooe/` folder. The `.obsidian/` directory in that folder carries the vault settings.

3. **Install Claude Code.** Follow the instructions at [claude.com/claude-code](https://claude.com/claude-code). Once installed, run `claude` from inside the inner `greenslaadttsooe/` folder so the assistant picks up `CLAUDE.md` automatically.

4. **Delete the contents of briefs, raw, and wiki.** Unless you want your wiki to include dragon and wizard references, of course.

5. **Add sources.** Drop any new source documents into `raw/` (or a subfolder of `raw/`). Then ask Claude to ingest them — it will follow the workflow defined in `CLAUDE.md`.

Nothing fancy. It's just Markdown.

## Folder structure

The repository root contains one working directory, `greenslaadttsooe/`, which is the Obsidian vault. Inside the vault:

- **`CLAUDE.md`** — instructions Claude Code reads on startup. Defines the ingest workflow, page format, citation rules, and lint behavior.
- **`ttsooe.md`** — the TTSOOE primer. Explains the teaching-as-marketing philosophy that drives every brief and wiki entry.
- **`readme.md`** — this file.
- **`raw/`** — source documents (articles, transcripts, notes). **Immutable.** Claude never modifies anything in here. Subfolders (e.g. `gse-calls/`, `gse-site/`) follow the same rule.
- **`wiki/`** — the knowledge base Claude maintains. One Markdown page per concept or source, connected by `[[wiki-links]]`. Contains three special files:
  - `index.md` — table of contents.
  - `log.md` — append-only record of every change.
  - `questions.md` — running list of audience questions you can (or should) answer.
- **`briefs/`** — content briefs Claude drafts on request. Each brief pulls from the wiki and follows the TTSOOE structure (problem → brand-agnostic teaching → why your solution).
- **`.obsidian/`** — Obsidian vault configuration. Safe to commit so collaborators get the same view.

## Usage

Typical sessions look like one of these:

- **Ingest a source.** Add a file to `raw/`, then ask Claude to ingest it. Claude summarizes the source, creates or updates concept pages in `wiki/`, links them together, and logs the change.
- **Ask the wiki a question.** Claude reads `wiki/index.md`, synthesizes an answer from relevant pages, and cites them. If the answer is valuable, Claude offers to save it back into the wiki.
- **Draft a content brief.** Claude pulls patterns from `wiki/` and writes a brief into `briefs/` following the TTSOOE structure.
- **Lint the wiki.** Claude checks for contradictions, orphan pages, missing concept pages, and format drift, then reports findings.

Full workflow rules live in [CLAUDE.md](CLAUDE.md).

## Contributing

This is a personal knowledge base rather than a shared codebase, so there's no formal contribution process. Fork it if you want to build your own version — the pattern transfers to any domain.

## License

Licensed under [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/)