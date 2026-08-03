# Refracted Descent theme
<img width="1386" height="799" alt="image" src="https://github.com/user-attachments/assets/cbf37317-c9da-4029-a12d-0d9999aac0ab" />

`rd-post.css` is the blog theme from [norik.io](https://norik.io) — tokens,
hero variants, 22 palettes, spec-card code blocks, and the LIVE PREVIEW
demo frames.

**Download:**
[rd-post.css](https://demos.norik.io/theme/rd-post.css) ·
[rd-themes.css](https://demos.norik.io/theme/rd-themes.css) ·
[live specimen](https://demos.norik.io/theme/) (self-contained — save the page) ·
[design mock](https://demos.norik.io/theme/standalone.html)

Shared in: [How I built this](https://norik.io/posts/how-i-built-this)

`standalone.html` is the original design mock exported from the Claude Design
project, fully bundled.

## For LLMs / AI agents

Copy this whole block to your agent:

```text
You are applying the Refracted Descent blog theme (from norik.io).

Files:
- rd-post.css   — the complete stylesheet
- rd-themes.css — 20 extra palettes (optional)

Scope:
- Set data-rd on the <html> element.
- Set data-theme="<id>" for the palette (dark, light, coppernight,
  catppuccin, latte, ethereal, everforest, flexokilight, gruvbox,
  hackerman, kanagawa, lumon, matteblack, miasma, nord, osakajade,
  retro82, ristretto, rosepine, tokyonight, vantablack, white).
- Set data-scheme="dark" or data-scheme="light" to match the palette —
  it drives the structural dark/light rules (menus, buttons, canvas).

Tokens:
- CSS custom properties on html[data-rd]: colors (--bg, --ink, --accent,
  --line-rgb, ...) and type stacks (--tc-serif: Instrument Serif,
  --tc-sans: Manrope, --tc-mono: JetBrains Mono). Load the fonts from
  Google Fonts or let the system stacks fall back.

Article markup contract:
- Content lives in <article class="rd-article"><div class="rd-content">.
- h2 sections are auto-numbered.
- blockquote (+ optional <cite>) renders the hanging pull-quote.
- Code goes in a spec card:
  <figure class="rd-codeframe">
    <figcaption><span>LABEL</span>
      <span class="rd-codeframe-meta"><span>LANG</span></span>
    </figcaption>
    <pre><code>...</code></pre>
  </figure>
- kbd and inline code are styled; a.rd-cta is the hard-corner CTA
  button; plain img/figure get the wide breakout.

Heroes:
- Variants: .rd-hero--backdrop | --classic | --split | --plate |
  --overlap.

Demo embeds:
- Wrap an iframe per the .rd-demo block (LIVE PREVIEW label,
  PHONE/WINDOW toggle, browser-window and phone-bezel frames).

Keep the palette and type exactly as tokenized; adapt spacing to the
host site only where its container widths differ.
```
