# drawio-skill — From Text to Professional Diagrams

[中文文档](README_CN.md) | [Online Docs](https://agents365-ai.github.io/drawio-skill/)

<p align="center">
  <img src="assets/workflow.png" width="420" alt="Workflow">
</p>

## What it does

| Capability | Description |
|---|---|
| `.drawio` XML generation | From natural-language descriptions |
| Multi-format export | PNG / SVG / PDF / JPG via the native draw.io desktop CLI |
| 6 diagram type presets | ERD, UML Class, Sequence, Architecture, ML/Deep Learning, Flowchart — preset shapes, styles, layout conventions |
| Animated connectors | `flowAnimation=1` for data-flow and pipeline diagrams (visible in SVG and draw.io desktop) |
| ML model diagrams | Tensor shape annotations `(B, C, H, W)` — ideal for NeurIPS/ICML/ICLR papers |
| Grid-aligned layout | All coordinates snap to 10px multiples for clean alignment |
| Browser fallback | Generates diagrams.net URLs when the desktop CLI is unavailable |
| Iterative design | Preview, gather feedback, refine until the diagram looks right |
| Auto-launch desktop | Opens draw.io after export for manual fine-tuning |
| Auto-trigger | Activates whenever diagrams would help explain complex systems |
| Style presets *(v1.3)* | Teach the skill your visual style from a `.drawio` file or image, save by name, reapply on demand |
| Custom output dir *(v1.4)* | Ask for any path (`./artifacts/`, `docs/images/`); the skill `mkdir -p`s and exports — ideal for CI/CD pipelines |

## Comparison

See [COMPARISON.md](COMPARISON.md) for side-by-side tables vs. native agents and vs. other draw.io skills/tools (jgraph/drawio-mcp, bahayonghang/drawio-skills, GBSOSS/ai-drawio), plus the key-advantages summary.

## Supported diagram types

| Category | Examples | Notable features |
|---|---|---|
| Architecture | microservices, cloud (AWS/GCP/Azure), network topology, deployment | Tier-based swimlanes, hub-center strategy |
| ML / Deep Learning | Transformer, CNN, LSTM, GRU | Tensor shape annotations, layer-type color coding |
| Flowcharts | business processes, workflows, decision trees, state machines | Semantic shapes (parallelogram I/O, diamond decisions) |
| UML | class diagrams, sequence diagrams | Inheritance / composition / aggregation arrows; lifelines + activation boxes |
| Data | ER diagrams, data flow diagrams (DFD) | Table containers, PK/FK notation |
| Other | org charts, mind maps, wireframes | — |

## Installation

Two steps — install the draw.io CLI first, then drop the skill into your host:

1. **[Install draw.io desktop](INSTALL_CLI.md)** — per-platform recipes for macOS / Windows / Linux.
2. **[Install the skill](INSTALL_SKILL.md)** — plugin marketplace (recommended), manual clone, and update commands.

## Usage

See [USAGE.md](USAGE.md) for natural-language prompts, a microservices walkthrough, and topology demos (star / layered / ring).

## Style Presets

See [STYLE_PRESETS.md](STYLE_PRESETS.md) for the built-in presets (`default` / `corporate` / `handdrawn`), the "learn my style from a file" workflow, and the full set of manage-presets commands.

## Support

If this skill helps you, consider supporting the author:

<table>
  <tr>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Agents365-ai/images_payment/main/qrcode/wechat-pay.png" width="180" alt="WeChat Pay">
      <br>
      <b>WeChat Pay</b>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Agents365-ai/images_payment/main/qrcode/alipay.png" width="180" alt="Alipay">
      <br>
      <b>Alipay</b>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Agents365-ai/images_payment/main/qrcode/buymeacoffee.png" width="180" alt="Buy Me a Coffee">
      <br>
      <b>Buy Me a Coffee</b>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/Agents365-ai/images_payment/main/awarding/award.gif" width="180" alt="Give a Reward">
      <br>
      <b>Give a Reward</b>
    </td>
  </tr>
</table>

## Author

**Agents365-ai**

- Bilibili: https://space.bilibili.com/441831884
- GitHub: https://github.com/Agents365-ai

## License

MIT
