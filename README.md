# WASM Blog

_This is showcase project for learning about WASM. Not to be considered production-ready._

The Goal is to make a static blog ready for web using rust compiled to wasm.

The article is in `./blog`.

Using `wasm_bindgen` and `pulldown-cmark` to render markdown on html.

```sh
.
├── Cargo.toml # Rust project configuration
├── blog # All Blog Posts
│   ├── post1.md
│   ├── post2.md
│   └── post3.md
├── index.html # Home page (entry point)
├── article.html # Template for individual blog articles
├── static/ # Static assets like CSS, images, or JavaScript
│   ├── style.css # Stylesheet for the blog
│   └── favicon.ico
├── target # auto-generated on build
├── pkg # auto-generated wasm binding (via `wasm-bindgen`)
│   ├── wasm_blog.d.ts
│   ├── wasm_blog.js
│   ├── wasm_blog_bg.wasm
│   └── wasm_blog_bg.wasm.d.ts
└── src
    ├── lib.rs # Main library file
    └── main.rs
```

In this part, the blog supports multiple articles and styling.
