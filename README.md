# reBot RK3576 LLM Grasp Docker Image

This repository publishes the RK3576 Docker image used for the reBot Arm B601-DM + Gemini336 LLM/typed-command grasping demo.

## Image

```bash
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:latest
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:rk3576-jazzy
docker pull ghcr.io/wrm119/rebot-rk3576-llm-grasp:20260611
```

## Main Project Path Inside Container

```text
/root/ros2_ws/src/rebot_grasp_llm
```

## Notes

- Target platform: Linux ARM64 / RK3576.
- Runtime environment: ROS2 Jazzy, RKNN Runtime, Orbbec SDK, reBot Python SDK.
- The image does not replace hardware-specific setup. Serial mapping, X11 authorization and hand-eye calibration still need to be checked on each new board.
