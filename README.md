# reBot RK3576 LLM Grasp Docker Image

This repository publishes the RK3576 Docker image used for the reBot Arm B601-DM + Gemini336 LLM/typed-command grasping demo.

## Public Download

Download the Docker image archive from the latest release:

```bash
curl -L -o rebot-rk3576-llm-grasp_20260611_arm64.docker.tar.gz https://github.com/wrm119/rebot-rk3576-llm-grasp/releases/download/v20260611/rebot-rk3576-llm-grasp_20260611_arm64.docker.tar.gz
gzip -dc rebot-rk3576-llm-grasp_20260611_arm64.docker.tar.gz | docker load
```

Loaded image tag:

```text
ghcr.io/wrm119/rebot-rk3576-llm-grasp:latest
```

## GHCR Tags

The image was also pushed to GitHub Container Registry:

```bash
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:latest
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:rk3576-jazzy
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:20260611
```

If GHCR package visibility is still private, use the public release archive above or change package visibility in GitHub Package settings.

## Main Project Path Inside Container

```text
/root/ros2_ws/src/rebot_grasp_llm
```

## Notes

- Target platform: Linux ARM64 / RK3576.
- Runtime environment: ROS2 Jazzy, RKNN Runtime, Orbbec SDK, reBot Python SDK.
- Hardware-specific setup is still required on each new board: serial mapping, X11 authorization and hand-eye calibration.
