# Konstantin Rusinevich (B34STW4RS)
### ML Engineer & Game Systems Architect

> **20 years of experience** bridging the gap between traditional game engines (C++/Unreal) and neural world models (PyTorch). Currently leading research on real-time neural rendering and ethical data synthesis.

---

## 01. Neural World Models & Inverse Dynamics (Proprietary Research)
*Note: The underlying architecture is proprietary. Below are outputs demonstrating the system's ability to synthesize worlds and infer control states. This was entirely a team effort, of some of the most talented people I ever had the pleasure to work with. Everything was trained on a single local 4090 for v1 and a single local 5090 for v2 and is capable of inference locally at 20fps on a single 4090 (imagine if we had the resources to go bigger.)*

### Phase 1: V1 Research Prototype
* **Goal:** Impressed by sudden emergence of world models, my team coalesced around the idea of creating our own proprietary version of the technology.
* **Constraint:** Optimized to train entirely on a single consumer GPU (RTX 4090).
* **Pipeline Optimization:** To solve training bottlenecks, we decoupled the data pipeline. We pre-encoded inputs and frames into tensor chunks, effectively splitting the process to maximize throughput.
* **Validation:** Initially benchmarked against Minecraft data to verify our novel architecture (distinct from SOTA), then validated on a barebones UE5 environment.

<table width="100%">
  <tr>
    <td align="center" width="50%"><b>Static / In-Place</b></td>
    <td align="center" width="50%"><b>Movement / Motion</b></td>
  </tr>
  <tr>
    <td valign="middle"><video src="https://github.com/user-attachments/assets/177aaa79-074d-4d43-9f49-d1c962d6e315" width="100%" controls></video></td>
    <td valign="middle"><video src="https://github.com/user-attachments/assets/1e7d3b27-7051-4d07-bce3-7c2ab7927b23" width="100%" controls></video></td>
  </tr>
</table>

<div align="center">
  <br>
  <b>V1 Inverse Dynamics Predictor</b><br>
  <em>Concept developed post-V2, demonstrated here running on the V1 architecture. This validated our ability to infer inputs from raw video, removing the strict requirement for ground-truth pairs <b>during training</b>.</em><br>
  <video src="https://github.com/user-attachments/assets/68b54e11-d3db-485c-a82e-4f35e666d61d" width="40%" controls></video>
  <br><br>
</div>

### Phase 2: V2 Increased Visual Fidelity
* **Goal:** To create our own ethical data source. This version used an expanded architecture in order to handle increased environment complexity.
* **Constraint:** Optimized to train entirely on a single RTX 5090 but still infer on a 4090.
* **Data Harvesting:** To solve data bottlenecks, we created bots with multiple views that could traverse our gameworld and capture 4x more data per bot.
* **Validation:** We learned that while our architecture was capable of learning effectively, it became very clear that there was an exponential need for more data.

<table width="100%">
  <tr>
    <td align="center" width="50%"><b>Static / In-Place</b></td>
    <td align="center" width="50%"><b>Movement / Motion</b></td>
  </tr>
  <tr>
    <td valign="middle"><video src="https://github.com/user-attachments/assets/26ef3ec2-d4a3-488a-bb38-0a86bd84cefb" width="100%" controls></video></td>
    <td valign="middle"><video src="https://github.com/user-attachments/assets/00696a0a-4e87-45e2-9f0d-a2be0391658e" width="100%" controls></video></td>
  </tr>
</table>

<div align="center">
  <br>
  <b>V2 Inverse Dynamics Predictor</b><br>
  <em>Refined inference handling our complex environment video data.</em><br>
  <video src="https://github.com/user-attachments/assets/a4527a2e-05b8-4cda-9f71-a108ead6fb3d" width="40%" controls></video>
  <br><br>
</div>

---

## 🧬 The "Data Factory": Ethical Data Lineage
To ensure 100% data ownership and avoid excessive web-scraping, we authored a custom "Data Laboratory" in Unreal Engine 5.

* **Process:** Automated agents navigate a custom-built 3D world to capture perfectly synchronized `Frame + Input` pairs.
* **Objective:** To train the Predictor on this ground-truth data, enabling future "zero-shot" auto-labeling of external video sources.

<div align="center">
  <video src="https://github.com/user-attachments/assets/5c1fbe1f-d0ee-4e49-b09d-94f6f0d776a3" width="100%" controls></video>
  <br>
  <em>Timelapse: Automated data harvesting in the synthetic UE5 environment.</em>
</div>

---

## 02. Experimental Game Dev (LLM-Assisted)
**Project:** Retro-Style Raycaster Engine
**Focus:** Benchmarking development velocity by using LLMs to port C++ rendering logic to monolithic HTML5/JS.
**Result:** A playable, pseudo-3D dungeon crawler built to test rapid prototyping workflows.

[ **Playable Demo** ](PASTE_YOUR_GAME_LINK_HERE)

<div align="center">
  <img src="PASTE_YOUR_RAYCASTER_SCREENSHOT_URL_HERE" width="100%" alt="Raycaster Demo">
</div>

---

## 03. Open Source Contribution
**Project:** [ComfyUI-itsB34ST-Nodes](https://github.com/B34STW4RS/ComfyUI-itsB34ST-Nodes)
**Focus:** Custom node systems for advanced generative workflows, including stylization and animation control.

<div align="center">
  <img src="PASTE_YOUR_COMFYUI_NODE_SCREENSHOT_URL_HERE" width="100%" alt="ComfyUI Workflow">
</div>

---

### Technical Toolbox
* **Languages:** Python, JavaScript/TypeScript, C++, HLSL
* **Machine Learning:** PyTorch, Custom Architecture Design, Synthetic Data Pipelines
* **Engines:** Unreal Engine 5, Custom Neural Renderers
* **Community:** Senior Moderator at **Banodoco** (ML Community)

<br>
<div align="center">
  <small>© 2026 Konstantin Rusinevich. All rights reserved. Media assets are strictly for demonstration purposes and remain the property of their respective owners.</small>
</div>
