[![tt-metal CI](https://github.com/tenstorrent/tt-metal/actions/workflows/all-post-commit-workflows.yaml/badge.svg)](https://github.com/tenstorrent/tt-metal/actions/workflows/all-post-commit-workflows.yaml)

<div align="center">

<h1>

[Bounty $](https://github.com/tenstorrent/tt-metal/issues?q=is%3Aissue%20state%3Aopen%20label%3Abounty) | [Buy](https://tenstorrent.com/cards/) | [Install](./INSTALLING.md) | [Discord](https://discord.gg/tvhGzHQwaj) | [Join Us](https://boards.greenhouse.io/tenstorrent/jobs/4155609007)

</h1>

<img src="https://github.com/user-attachments/assets/a67452e7-e310-4c90-9a0c-a823efb20c74" alt="ttnn logo" height="180"/>

**TT-NN** is a Python & C++ Neural Network OP library.

<h3>

[API Reference](https://docs.tenstorrent.com/tt-metal/latest/ttnn/index.html) | [Model Demos](./models/demos/)

</h3>

</div>

# Tenstorrent Model Performance Overview

---

## 🚀 Top 3 Models on **Wormhole** (WH)

| Model          | March '25 | April '25 | May '25 (Latest) |
|----------------|-----------|-----------|------------------|
| LLaMA 2 70B    | 22 tok/s  | 26 tok/s  | **29 tok/s**     |
| Mistral 7B     | 45 tok/s  | 50 tok/s  | **53 tok/s**     |
| Stable Diffusion 2 | 13 img/s | 16 img/s | **18 img/s**     |

👉 **For full model support, demos, and performance history, visit [Complete Demos & Metrics](./models/demos)**

<h3>🚀 Top 3 Models on Wormhole (WH)</h3>

<table>
  <thead>
    <tr>
      <th align="left">Model</th>
      <th>Progress</th>
      <th align="center">Latest Perf</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>LLaMA 2 70B</b></td>
      <td>
        <div style="display:flex;gap:4px;align-items:flex-end;height:60px;">
          <div style="width:12px;height:25px;background:#bbb;border-radius:2px;"></div>
          <div style="width:12px;height:35px;background:#888;border-radius:2px;"></div>
          <div style="width:12px;height:45px;background:#333;border-radius:2px;"></div>
        </div>
      </td>
      <td align="center"><b>29 tok/s</b></td>
    </tr>
    <tr>
      <td><b>Mistral 7B</b></td>
      <td>
        <div style="display:flex;gap:4px;align-items:flex-end;height:60px;">
          <div style="width:12px;height:40px;background:#bbb;border-radius:2px;"></div>
          <div style="width:12px;height:47px;background:#888;border-radius:2px;"></div>
          <div style="width:12px;height:53px;background:#333;border-radius:2px;"></div>
        </div>
      </td>
      <td align="center"><b>53 tok/s</b></td>
    </tr>
    <tr>
      <td><b>Stable Diffusion 2</b></td>
      <td>
        <div style="display:flex;gap:4px;align-items:flex-end;height:60px;">
          <div style="width:12px;height:20px;background:#bbb;border-radius:2px;"></div>
          <div style="width:12px;height:30px;background:#888;border-radius:2px;"></div>
          <div style="width:12px;height:38px;background:#333;border-radius:2px;"></div>
        </div>
      </td>
      <td align="center"><b>18 img/s</b></td>
    </tr>
  </tbody>
</table>

---

## 🧠 First Results on **Blackhole** (BH)

| Model            | March '25 | April '25 | May '25 (Latest) |
|------------------|-----------|-----------|------------------|
| LLaMA 3.3 8B     | 110 tok/s | 125 tok/s | **140 tok/s**    |

👉 **Explore the full Blackhole lineup and benchmarks [here](./models/demos/Blackhole)**

---

# 📂 Model Demos and Performance Breakdown

Models are now structured by **platform** and **task category**, inspired by HuggingFace model tags.

### 🔹 Wormhole

```
models/demos/Wormhole/
├── Text Generation/
├── Text-to-Image/
├── Image-Text-to-Text/
├── Feature Extraction/
├── ...
```

### 🔹 Blackhole

```
models/demos/Blackhole/
├── Text Generation/
│   └── LLaMA 3.3 8B/
├── Text-to-Image/
├── Text-to-Video/
├── ...
```

Each category includes:
- A `README.md` summarizing supported models, metrics, supported ops, and perf history
- Demo scripts and instructions for running on Tenstorrent hardware

---

## 🧭 Navigation

- [All Wormhole Demos](./models/demos/Wormhole)
- [All Blackhole Demos](./models/demos/Blackhole)
- [Transformer Library (tt_transformers)](./models/tt_transformers)

For contributing new models or perf data, please open a PR or file an issue tagged `model-benchmark`.

---

🔔 **Note:** This repo is under active reorganization. Please ensure you're referencing the latest folders and documentation.

---

Made with ❤️ by the Tenstorrent AI Team
