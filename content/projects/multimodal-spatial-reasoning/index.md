---
title: Multimodal Spatial Reasoning & Object Memory
summary: Lightweight object-centric semantic 3D memory for wearable and embodied spatial intelligence.
date: 2026-01-01
featured: true
weight: 5
tags:
  - Robotics
  - Multimodal AI
  - Spatial Reasoning
  - Embodied Agents
---

I am developing lightweight object-centric semantic 3D memory for wearable and embodied spatial intelligence. The system converts sparse egocentric RGB/depth/pose observations into localized object records, so an agent can answer spatial queries without storing or processing every frame as a dense map.

**Current pipeline**
- Sparse Habitat/HM3D or egocentric exploration with VLM-guided object-category selection.
- YOLO-World detection, NanoSAM masks, DepthPro depth, field-of-view geometry, and visibility-aware object scoring.
- Batched or crop-level object VLM descriptions, CLIP/DINOv3 embeddings, and cross-view association.
- Queryable object records with labels, masks, depth, global coordinates, object-view links, and object-object spatial relations.
- Wearable/robot-side object memory with edge/cloud support for heavier perception, identity consolidation, and prioritized map updates.

**Supported tasks**
- View retrieval, object localization, instance clustering, and spatial search.
- Agentic grounding for robots or wearable assistants operating under sensing, power, bandwidth, and compute constraints.
