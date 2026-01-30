# Konstantin Rusinevich (B34STW4RS)
### ML Engineer & Game Systems Architect

> **20 years of experience** bridging the gap between traditional game engines (C++/Unreal) and neural world models (PyTorch). Currently leading research on real-time neural rendering and ethical data synthesis.

---

## 01. Neural World Models & Inverse Dynamics (Proprietary Research)
*Note: The underlying architecture is proprietary. Below are outputs demonstrating the system's ability to synthesize worlds and infer control states.*

### Phase 1: V1 Research Prototype
**Goal:** Establishing latent manifold stability and mapping fundamental movement deltas to synthesized frame transitions.

<table width="100%">
  <tr>
    <td align="center" width="50%"><b>Static / In-Place</b></td>
    <td align="center" width="50%"><b>Movement / Motion</b></td>
  </tr>
  <tr>
    <td><video src="https://github.com/user-attachments/assets/177aaa79-074d-4d43-9f49-d1c962d6e315" width="100%" controls></video></td>
    <td><video src="https://github.com/user-attachments/assets/1e7d3b27-7051-4d07-bce3-7c2ab7927b23" width="100%" controls></video></td>
  </tr>
</table>

<p align="center">
  <b>V1 Inverse Dynamics Predictor</b><br>
  <em>Reconstructing control vectors (x, y, z) from latent shifts.</em><br>
  <video src="https://github.com/user-attachments/assets/68b54e11-d3db-485c-a82e-4f35e666d61d" width="60%" controls></video>
</p>

### Phase 2: V2 High-Fidelity Iteration
**Goal:** Increased environment complexity and temporal persistence. This version handles rotational data and non-linear acceleration within the synthesized world.

<table width="100%">
  <tr>
    <td align="center" width="50%"><b>Static / In-Place</b></td>
    <td align="center" width="50%"><b>Movement / Motion</b></td>
  </tr>
  <tr>
    <td><video src="https://github.com/user-attachments/assets/26ef3ec2-d4a3-488a-bb38-0a86bd84cefb" width="100%" controls></video></td>
    <td><video src="https://github.com/user-attachments/assets/00696a0a-4e87-45e2-9f0d-a2be0391658e" width="100%" controls></video></td>
  </tr>
</table>

<p align="center">
  <b>V2 Inverse Dynamics Predictor</b><br>
  <em>Refined inference handling complex rotational data.</em><br>
  <video src="https://github.com/user-attachments/assets/a4527a2e-05b8-4cda-9f71-a108ead6fb3d" width="60%" controls></video>
</p>

---

## 🧬 The "Data Factory": Ethical Data Lineage
To ensure 100% data ownership and avoid web-scraping, we authored a custom "Data Laboratory" in Unreal Engine 5.

* **Process:** Automated agents navigate a custom-built 3D world to capture perfectly synchronized `Frame + Input` pairs.
* **Objective:** To train the Predictor on this ground-truth data, enabling future "zero-shot" auto-labeling of external video sources.

<p align="center">
  <video src="https://github.com/user-attachments/assets/5c1fbe1f-d0ee-4e49-b09d-94f6f0d776a3" width="100%" controls></video>
  <br>
  <em>Timelapse: Automated data harvesting in the synthetic UE5 environment.</em>
</p>

---

## 02. Experimental Game Dev (LLM-Assisted)
**Project:** Retro-Style Raycaster Engine
**Focus:** Benchmarking development velocity by using LLMs to port C++ rendering logic to monolithic HTML5/JS.
**Result:** A playable, pseudo-3D dungeon crawler built to test rapid prototyping workflows.

[ **Playable Demo** ](PASTE_YOUR_GAME_LINK_HERE)

<p align="center">
  <img src="PASTE_YOUR_RAYCASTER_SCREENSHOT_URL_HERE" width="100%" alt="Raycaster Demo">
</p>

---

## 03. Open Source Contribution
**Project:** [ComfyUI-itsB34ST-Nodes](https://github.com/B34STW4RS/ComfyUI-itsB34ST-Nodes)
**Focus:** Custom node systems for advanced generative workflows, including stylization and animation control.

<p align="center">
  <img src="PASTE_YOUR_COMFYUI_NODE_SCREENSHOT_URL_HERE" width="100%" alt="ComfyUI Workflow">
</p>

---

### Technical Toolbox
* **Languages:** Python, JavaScript/TypeScript, C++, HLSL
* **Machine Learning:** PyTorch, Custom Architecture Design, Synthetic Data Pipelines
* **Engines:** Unreal Engine 5, Custom Neural Renderers
* **Community:** Senior Moderator at **Banodoco** (ML Community)


© 2026 Konstantin Rusinevich. All rights reserved. Media assets are strictly for demonstration purposes and remain the property of their respective owners.
