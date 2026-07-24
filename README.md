# Learning Business Central

Static site published with GitHub Pages: `https://rcorella.github.io/LearningBusinessCentral/`

## Structure

```
.
├── index.html                              # Home page — lists all posts
├── posts/
│   └── agentic-development-instructions.html
├── assets/
│   ├── css/
│   │   └── style.css                       # Shared stylesheet, all pages import this
│   └── images/                             # Local copies of post images (optional, see below)
└── README.md
```

Content pages live under `posts/`, styling is centralized in `assets/css/style.css`, so nothing is duplicated at the root — the root only holds `index.html` as the entry point GitHub Pages expects.

## Adding a new post

1. Duplicate `posts/agentic-development-instructions.html` as a starting template.
2. Update the `<title>`, `<meta name="description">`, `<h1>`, `.meta` line, and body content.
3. Add a `<li class="post-card">` entry to `index.html` linking to the new file.
4. Commit and push to `main` — GitHub Pages rebuilds automatically.

## Images

The current post links directly to the images already hosted on the original blog post (`blog.msdyn365bc.es`). If you'd rather host them inside this repo (recommended for full independence from the original blog), download them into `assets/images/` and update the `src` attributes in the post to relative paths, e.g. `../assets/images/instructions-example.png`.

## GitHub Pages configuration

Settings → Pages → Source: **Deploy from a branch** → Branch: **main** → Folder: **/ (root)**.
