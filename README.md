# Vision World Models for Manufacturing & Industrial Automation

**From Seeing the Factory to Predicting What Happens Next**

Curated GitHub repositories for the six core concepts and nine applications in the *Vision World Models* infographic, plus a compact catalog you can clone and extend.

[![Repo](https://img.shields.io/badge/github-vision--world--models--manufacturing-blue)](https://github.com/ahmaddroobi99/vision-world-models-manufacturing)
[![Concepts](https://img.shields.io/badge/core_concepts-6-informational)](docs/01-core-concepts.md)
[![Apps](https://img.shields.io/badge/applications-9-informational)](docs/02-applications.md)
[![Repos](https://img.shields.io/badge/~35_repos-per_category-success)](#catalog)

## Pipeline

```mermaid
flowchart LR
  SEE[See] --> UND[Understand]
  UND --> PRED[Predict]
  PRED --> SIM[Simulate]
  SIM --> PLAN[Plan]
  PLAN --> ACT[Act]
```

| Stage | Question the plant is asking |
|---|---|
| See | What is on the line right now? |
| Understand | Where is everything in 3D, and who is moving? |
| Predict | What state, failure, or collision comes next? |
| Simulate | What happens if the robot takes this action? |
| Plan | Which action is safest and most productive? |
| Act | Execute, then watch the world update. |

## Repo layout

| Path | Purpose |
|---|---|
| [docs/01-core-concepts.md](docs/01-core-concepts.md) | 6 foundation stacks — ~35 repos each |
| [docs/02-applications.md](docs/02-applications.md) | 9 factory applications — ~35 repos each |

## The 6 core concepts

| # | Concept | Flagship models | Role |
|---|---|---|---|
| 1 | Scene Representation | ViT / DINOv2 / DINOv3 | Machines, parts, tools, workers as one scene |
| 2 | Spatial Understanding | Depth Anything / VGGT | 3D pose, depth, clearance, free space |
| 3 | Dynamics & Motion | VideoMAE / CoTracker | How product, robot, and worker move |
| 4 | Future Prediction | V-JEPA / Video Transformer | Upcoming states, failures, collisions |
| 5 | Action Simulation | DreamerV3 / Diffusion Policy | Imagine actions before they run |
| 6 | Planning & Action | VLA / OpenVLA / π₀ | Choose and execute the next move |

Hubs: [DINOv2](https://github.com/facebookresearch/dinov2) · [DINOv3](https://github.com/facebookresearch/dinov3) · [VGGT](https://github.com/facebookresearch/vggt) · [Depth Anything V2](https://github.com/DepthAnything/Depth-Anything-V2) · [CoTracker](https://github.com/facebookresearch/co-tracker) · [V-JEPA 2](https://github.com/facebookresearch/vjepa2) · [DreamerV3](https://github.com/danijar/dreamerv3) · [Diffusion Policy](https://github.com/real-stanford/diffusion_policy) · [OpenVLA](https://github.com/openvla/openvla) · [openpi](https://github.com/Physical-Intelligence/openpi) · [LeRobot](https://github.com/huggingface/lerobot)

## The 9 applications

| # | Application | What the world model is for |
|---|---|---|
| 1 | Adaptive Robotic Assembly | Predict how parts will interact during insertion |
| 2 | Intelligent Pick & Place | Simulate grasps, keep the safest one |
| 3 | Predictive Quality Inspection | See defects forming in image + process traces |
| 4 | Predictive Maintenance | Anticipate abnormal machine states |
| 5 | Human–Robot Collaboration | Predict worker motion, slow or replan |
| 6 | Production-Line Optimization | Forecast downstream effects of a change |
| 7 | Autonomous Material Handling | Predict dynamic obstacles, move safely |
| 8 | Process Anomaly Prediction | Catch deviations before they become scrap |
| 9 | Flexible Manufacturing | Retask when SKU, layout, or process changes |

Hubs reused across applications on purpose: [anomalib](https://github.com/open-edge-platform/anomalib) · [Isaac Lab](https://github.com/isaac-sim/IsaacLab) · [cuRobo](https://github.com/NVlabs/curobo) · [MoveIt 2](https://github.com/moveit/moveit2) · [SAM 2](https://github.com/facebookresearch/sam2) · [YOLO](https://github.com/ultralytics/ultralytics) · [Nav2](https://github.com/ros-navigation/navigation2) · [Open-RMF](https://github.com/open-rmf/rmf) · [NVIDIA Cosmos](https://github.com/NVIDIA/Cosmos)

## Catalog

See the two docs for the full ~35-repo lists. Flagship one-liners:

### Concepts
1. Scene — [dinov2](https://github.com/facebookresearch/dinov2) · [dinov3](https://github.com/facebookresearch/dinov3) · [timm](https://github.com/huggingface/pytorch-image-models) · [SAM 2](https://github.com/facebookresearch/sam2)
2. Spatial — [VGGT](https://github.com/facebookresearch/vggt) · [VGGT-Omega](https://github.com/facebookresearch/vggt-omega) · [Depth Anything V2](https://github.com/DepthAnything/Depth-Anything-V2) · [Depth Anything 3](https://github.com/ByteDance-Seed/Depth-Anything-3)
3. Dynamics — [CoTracker](https://github.com/facebookresearch/co-tracker) · [VideoMAE](https://github.com/MCG-NJU/VideoMAE) · [TAPIR](https://github.com/google-deepmind/tapnet) · [RAFT](https://github.com/princeton-vl/RAFT)
4. Future — [V-JEPA 2](https://github.com/facebookresearch/vjepa2) · [V-JEPA](https://github.com/facebookresearch/jepa) · [Cosmos](https://github.com/NVIDIA/Cosmos) · [InternVideo2](https://github.com/OpenGVLab/InternVideo2)
5. Simulate — [DreamerV3](https://github.com/danijar/dreamerv3) · [Diffusion Policy](https://github.com/real-stanford/diffusion_policy) · [TD-MPC2](https://github.com/nicklashansen/tdmpc2) · [Isaac Lab](https://github.com/isaac-sim/IsaacLab)
6. Plan/Act — [OpenVLA](https://github.com/openvla/openvla) · [openpi](https://github.com/Physical-Intelligence/openpi) · [GR00T](https://github.com/NVIDIA/Isaac-GR00T) · [LeRobot](https://github.com/huggingface/lerobot)

### Applications
1. Assembly — [IndustReal lib](https://github.com/NVlabs/industreallib) · [Factory](https://github.com/NVlabs/Factory) · [cuRobo](https://github.com/NVlabs/curobo) · [FurnitureBench](https://github.com/clvrai/furniture-bench)
2. Pick & place — [AnyGrasp](https://github.com/graspnet/anygrasp_sdk) · [Contact-GraspNet](https://github.com/NVlabs/contact_graspnet) · [GraspNet](https://github.com/graspnet/graspnet-baseline)
3. Quality — [anomalib](https://github.com/open-edge-platform/anomalib) · [PatchCore](https://github.com/amazon-science/patchcore-inspection) · [EfficientAD](https://github.com/nelson1425/EfficientAD)
4. Maintenance — [anomalib](https://github.com/open-edge-platform/anomalib) · [Time-Series-Library](https://github.com/thuml/Time-Series-Library) · [V-JEPA 2](https://github.com/facebookresearch/vjepa2)
5. HRC — [MMPose](https://github.com/open-mmlab/mmpose) · [cuRobo](https://github.com/NVlabs/curobo) · [MoveIt 2](https://github.com/moveit/moveit2)
6. Line opt — [Isaac Lab](https://github.com/isaac-sim/IsaacLab) · [OR-Tools](https://github.com/google/or-tools) · [Open-RMF](https://github.com/open-rmf/rmf)
7. Material handling — [Nav2](https://github.com/ros-navigation/navigation2) · [nvblox](https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_nvblox) · [Open-RMF](https://github.com/open-rmf/rmf)
8. Process anomaly — [anomalib](https://github.com/open-edge-platform/anomalib) · [TranAD](https://github.com/imperial-qore/TranAD) · [ruptures](https://github.com/deepcharles/ruptures)
9. Flexible MFG — [OpenVLA](https://github.com/openvla/openvla) · [openpi](https://github.com/Physical-Intelligence/openpi) · [LeRobot](https://github.com/huggingface/lerobot)

## Selection policy

Official paper code first, then widely used toolboxes, datasets/eval kits, simulators, and industrial CV / ROS 2 stacks. Abandoned one-off forks excluded. Shared hubs (DINOv2, SAM 2, YOLO, cuRobo, Isaac Lab, anomalib, LeRobot) appear under multiple topics on purpose. Star counts are snapshots from around 2026-09-05.

## License

Documentation in this repository is for research navigation. Linked projects keep their own licenses.
