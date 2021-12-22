+++
title = "KaTeX - Rust"
weight = 0
summary = "Render math formulas using KaTeX - written in Rust"

repository = "https://github.com/grego/blades-katex-rs"
+++
Blades natively supports rendering LaTeX formulas into [MathML](https://developer.mozilla.org/docs/Web/MathML).
Sadly, Chromium-based browsers don't support it.
This plugin renders the formulas into HTML using [KaTeX](https://katex.org),
run with the QuickJS enginge.
Formulas delimited by `$` are rendered in inline mode and by `$$` in display mode.

This plugin can be installed as
```bash
cargo install blades-katex
```

Then, it can be used in Blades as
```toml
[plugins.content]
katex = "blades-katex"
```

On each page where KaTeX should be rendered, it can be enabled by
```toml
plugins = ["katex"]
```
