# Getting Started with ScrollWorkflows 🚀

Welcome to ScrollWorkflows. This guide covers how to set up your environment, connect your nodes, and run your first toolkit pipeline.

## 1. Prerequisites

Before importing workflows, ensure you have access to:
- **ComfyUI:** Installed locally or running on a cloud GPU (e.g. RunPod, Vast.ai).
- **n8n:** Self-hosted instance or n8n Cloud for orchestration.
- **API Keys:** Hugging Face token (for model downloads), OpenAI or Claude API key (for agentic scriptwriting).

## 2. Choosing a Toolkit

ScrollWorkflows provides three primary plug-and-play workflows:
- **Image → Ads:** Generates multi-angle product assets from a single input photo.
- **AI Influencer:** Consistent character rendering with LoRA weights, facial landmark alignment, and skin detailers.
- **Mini Series:** Multi-scene storytelling workflows combining text-to-speech, LipSync, and video synthesis.

## 3. Workflow Import Process

1. Download the workflow `.json` file from your ScrollWorkflows dashboard.
2. In **ComfyUI**, drag and drop the `.json` file into the canvas.
3. Install any missing custom nodes via **ComfyUI-Manager** by clicking **"Install Missing Custom Nodes"**.
4. Restart ComfyUI to reload newly compiled python modules.
5. In **n8n**, click **Workflows → Import from File** to load the automation triggers and webhook handlers.

## 4. Need Help?

Join our community discord or open an issue on the repository if you encounter missing custom node definitions.


