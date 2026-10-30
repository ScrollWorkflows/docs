# RunPod GPU Deployment Guide ☁️

This guide explains how to run ScrollWorkflows on cloud GPUs via RunPod for high-performance rendering.

## Recommended GPU Specifications

| Workflow Tier | Recommended GPU | VRAM |
|---|---|---|
| Image → Ads (SDXL / Flux Schnell) | RTX 4090 / A5000 | 24 GB |
| AI Influencer (LoRA + FaceDetailer) | RTX 4090 / A6000 | 24 GB - 48 GB |
| Mini Series (Video Synthesis + LipSync) | A100 (80GB) / H100 | 80 GB |

## 1. Network Volume Setup

To avoid re-downloading model checkpoints every session:
1. Navigate to **Storage → Network Volumes** in your RunPod dashboard.
2. Create a volume (e.g. `scroll-models`, 100 GB).
3. Mount the volume under `/workspace` when spinning up your pod.

## 2. Deploying the ComfyUI Template

1. Under **Community Templates**, search for `runpod/comfyui` or use the official ScrollWorkflows template.
2. Set environment variables for your Hugging Face and CivitAI API keys.
3. Expose HTTP ports `8188` (ComfyUI Web UI) and `22` (SSH).
4. Launch the instance and connect through the direct web interface link.
