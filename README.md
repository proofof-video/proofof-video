# Proof of Video

**[proofof.video](https://proofof.video)** — A community gallery comparing state-of-the-art AI/LLM-generated **interactive, explorable 3D worlds** side-by-side.

Same (or similar) prompts. Different models. Different software. Real video output.

> **Scope:** This project focuses on **interactive, explorable 3D worlds and simulations** — not linear video or film. Pure video-generation tools (e.g. text-to-video models that output flat MP4s without an explorable 3D scene) do not qualify.

## What Is This?

AI tools can now generate interactive 3D worlds, physics simulations, and explorable scenes from plain text prompts. But how do they actually compare? This project is a transparent, community-driven benchmark — a gallery where anyone can submit a video of an **explorable 3D world** they generated and see it alongside results from other models and tools using the same prompt.

Inspired by projects like:
- [LocalGPT-Gen](https://github.com/localgpt-app/localgpt)
- [Blender MCP](https://github.com/ahujasid/blender-mcp)
- [Genesis Embodied AI](https://genesis-embodied-ai.github.io/)

## How to Contribute

1. Run a prompt through your chosen LLM + 3D software pipeline
2. Upload the result to YouTube
3. Add an entry `.md` file in the `_entries/` folder (see [CONTRIBUTING.md](CONTRIBUTING.md) for the simple template)
4. Open a Pull Request

All skill levels and tools are welcome. The more data points, the richer the comparison.

## Local Development

This site uses Jekyll with the `github-pages` gem to match GitHub Pages' build environment.

### Prerequisites

- Ruby 3.3.x (managed via [mise](https://mise.jdx.dev/) or similar)
- Bundler

### Setup

```bash
# Install Ruby 3.3 (if using mise)
mise install ruby@3.3

# Install dependencies
bundle install

# Start local server with live reload
bundle exec jekyll serve --livereload
```

The site will be available at http://127.0.0.1:4000

### Ruby Version

GitHub Pages currently uses Ruby 3.3.4. This project is configured for Ruby 3.3.x via `mise.toml` to ensure compatibility with the `github-pages` gem (v232) and its dependencies.

## Site Structure

```
index.html          ← Main gallery page (auto-rendered from entries)
_entries/           ← One .md file per video submission
assets/css/         ← Styles (no framework, plain CSS)
CNAME               ← Custom domain: proofof.video
_config.yml         ← GitHub Pages / Jekyll config
CONTRIBUTING.md     ← How to add your video
```

## License

[Apache 2.0](LICENSE)
