---
title: Multimodal Spatial Reasoning & Object Memory
summary: Object-centric graph memories for view retrieval, object localization, instance clustering, object search, and agentic robot grounding.
date: 2026-01-01
featured: true
weight: 5
tags:
  - Robotics
  - Multimodal AI
  - Spatial Reasoning
  - Embodied Agents
---

I am developing a spatial-reasoning pipeline that converts Habitat exploration into object-level graph memories by fusing detector masks, depth geometry, VLM descriptions, and CLIP/DINOv3 representations. The pipeline supports view retrieval, object localization, instance clustering, object search, and agentic robot grounding.

**Current pipeline**
- Habitat exploration with VLM-based object-category selection.
- YOLO-World detection, NanoSAM masks, DepthPro depth, and geometric projection.
- Batched or crop-level object VLM descriptions.
- CLIP/DINOv3 object embeddings and spatial database artifacts.
- View retrieval, object localization, instance clustering, and analysis.
