# donghui-0126.github.io

Personal portfolio site — **[donghui-0126.github.io](https://donghui-0126.github.io)**

Single-page, minimal light theme. Crypto quant research, HFT systems
engineering, and LLM-driven research infrastructure.

## How it works (markdown-driven, no build step)

- **`content.md`** — the actual page content. Edit this and commit; the live
  site renders it immediately (client-side via [marked](https://marked.js.org)).
- **`index.html`** — thin shell: fonts, styles, nav/footer, and the renderer
  that fetches `content.md` and injects it.
- Most content is plain **Markdown** (headings, lists, tables, links). The
  rich components (Journey timeline, Project cards, Engineering cards) are
  small **HTML blocks** kept inside `content.md` — edit the text, leave the
  structure. Section headers `<h2 id="...">` are anchored to the nav; keep the ids.
- Deployed via GitHub Pages from the `main` branch (`.nojekyll` present).

To update the site: edit `content.md` → commit → push. Done.

📫 lukedonghui@gmail.com
