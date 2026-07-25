# Jamez’s Blog

Hugo site source for a technical blog about large language models, inference systems, and AI products.

## Local development

Install Hugo `0.164.0` or newer, then initialize the theme and start the development server:

```bash
git submodule update --init --recursive
hugo server --buildDrafts
```

Open <http://localhost:1313/>.

The `content/posts/dev-*` page bundles are draft-only fixtures for checking article cards, covers, search, math, code highlighting, tables, and the H2/H3 table of contents. A normal production build excludes them:

```bash
hugo --gc --minify
```

Before deployment, set `baseURL` in `hugo.yaml` to the final site URL.
