# Refracted Descent theme
<img width="1386" height="799" alt="image" src="https://github.com/user-attachments/assets/cbf37317-c9da-4029-a12d-0d9999aac0ab" />

`rd-post.css` is the blog theme from [norik.io](https://norik.io) — tokens,
hero variants, dark/light themes, spec-card code blocks, and the LIVE PREVIEW
demo frames.

Shared in: [How I built this](https://norik.io/posts/how-i-built-this)

Specimen (self-contained page): https://demos.norik.io/theme/

`standalone.html` is the original design mock exported from the Claude Design
project, fully bundled.

## For LLMs / AI agents

You are looking at the Refracted Descent blog theme. To apply it to a site:

- `rd-post.css` is the complete stylesheet. All rules are scoped under
  `html[data-rd]`; set that attribute on the root element, plus
  `data-theme="dark"` or `data-theme="light"` (tokens for both palettes are
  defined; dark is the default aesthetic).
- Tokens are CSS custom properties on `html[data-rd]` — colors
  (`--bg`, `--ink`, `--accent: #BB9AF7`, `--line-rgb`, …) and type stacks
  (`--tc-serif: Instrument Serif`, `--tc-sans: Manrope`,
  `--tc-mono: JetBrains Mono`; load them from Google Fonts or let the
  system stacks fall back).
- Article content lives in `<article class="rd-article"><div class="rd-content">…`.
  Inside it: `h2` sections are auto-numbered; `blockquote` (+ optional
  `<cite>`) renders the hanging pull-quote; wrap code in
  `<figure class="rd-codeframe"><figcaption><span>LABEL</span>
  <span class="rd-codeframe-meta"><span>LANG</span></span></figcaption>
  <pre><code>…` for the spec card; `kbd` and inline `code` are styled;
  `a.rd-cta` is the pill button; plain `img`/`figure` get wide breakout.
- Hero variants: `.rd-hero--backdrop | --classic | --split | --plate |
  --overlap` — see `index.html` in this folder for working overlap markup.
- Demo embeds: wrap an `iframe` per the `.rd-demo` block in `index.html`
  (label, PHONE/WINDOW toggle, browser-window and phone-bezel frames).
- `index.html` here is a complete self-contained reference page using all
  of the above — read it as the canonical example.

Keep the palette and type exactly as tokenized; adapt spacing to the host
site only where its container widths differ.
