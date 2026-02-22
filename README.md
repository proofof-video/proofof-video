# Proof of Video

**[proofof.video](https://proofof.video)** — A community gallery comparing state-of-the-art AI/LLM-generated 3D worlds side-by-side.

Same (or similar) prompts. Different models. Different software. Real video output.

## What Is This?

AI tools can now generate 3D worlds, physics simulations, and cinematic scenes from plain text prompts. But how do they actually compare? This project is a transparent, community-driven benchmark — a gallery where anyone can submit a video they generated and see it alongside results from other models and tools using the same prompt.

Inspired by projects like:
- [LocalGPT-Gen](https://github.com/localgpt-app/localgpt)
- [Blender MCP](https://github.com/ahujasid/blender-mcp)
- [Genesis Embodied AI](https://genesis-embodied-ai.github.io/)

## How to Contribute

1. Run a prompt through your chosen LLM + 3D software pipeline
2. Upload the result to YouTube
3. Add a video card to `index.html` (see [CONTRIBUTING.md](CONTRIBUTING.md) for the exact template)
4. Open a Pull Request

All skill levels and tools are welcome. The more data points, the richer the comparison.

## Site Structure

```
index.html          ← Main gallery page
assets/css/         ← Styles (no framework, plain CSS)
CNAME               ← Custom domain: proofof.video
_config.yml         ← GitHub Pages config
CONTRIBUTING.md     ← How to add your video
```

## License

[MIT](LICENSE)
