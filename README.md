# <img src="assets/logo/pov.svg" alt="logo" width="32" height="32"> Proof of Video

**[proofof.video](https://proofof.video)** — A community gallery comparing state-of-the-art AI/LLM-generated **interactive, explorable worlds** (2D and 3D) side-by-side.

Same (or similar) prompts. Different models. Different software. Real video output.

> **Scope:** This project focuses on **interactive, explorable worlds** (2D and 3D) — not linear video or film. Pure video-generation tools (e.g. text-to-video models that output flat MP4s without an explorable world) do not qualify.

## What Is This?

AI tools can now generate interactive 2D and 3D worlds and explorable scenes from plain text prompts. But how do they actually compare? This project is a transparent, community-driven benchmark — a gallery where anyone can submit a video of an **explorable world** they generated and see it alongside results from other models and tools using the same prompt.

Inspired by projects like:
- [LocalGPT-Gen](https://github.com/localgpt-app/localgpt)
- [Blender MCP](https://github.com/ahujasid/blender-mcp)
- [Genesis Embodied AI](https://genesis-embodied-ai.github.io/)

## How to Contribute

1. Run a prompt through your chosen LLM + software pipeline
2. Upload the result to YouTube
3. Add an entry `.md` file in the `_entries/` folder (see [CONTRIBUTING.md](CONTRIBUTING.md) for the simple template)
4. Open a Pull Request

All skill levels and tools are welcome. The more data points, the richer the comparison.

## Local Development

This site uses Jekyll with the `github-pages` gem to match GitHub Pages' build environment. [mise](https://mise.jdx.dev/) manages Ruby and provides dev tasks.

### Setup

```bash
# Install Ruby 3.3.4 (pinned to match GitHub Pages)
mise install

# Install dependencies
mise run install

# Start local server with live reload
mise run serve
```

The site will be available at http://127.0.0.1:4000

### Available Tasks

| Command | Description |
|---------|-------------|
| `mise run install` | Install Ruby dependencies |
| `mise run serve` | Start Jekyll with live reload |
| `mise run build` | Build the site to `_site/` |

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
