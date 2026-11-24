# Holographic View

Use Holographic View to inspect the robot model and observe how joint feedback updates its live pose. The information available depends on the model and feedback published by your project.

## Model Inspection

1. Open the Holographic View and switch to **Model Inspection**.
2. Load or select the robot model available to the view. Inspect the model and identify where the sensor and actuator markers sit relative to the links and joints.
3. Use the model view to understand the robot's layout before following live motion. The upward lighting sweep is part of this inspection mode.

## Live Kinematics

1. Launch your robot or simulation and use its ROS connection in the workbench.
2. Switch to **Live Kinematics**.
3. Move a joint in simulation or use an existing simulation sequence. Watch the corresponding joint in the model and compare it with the joint feedback published by the project.

| Indicator | Meaning |
| --- | --- |
| Sensor marker | Identifies a sensor position. The marker color identifies the marker type. |
| Blue actuator marker | Normal actuator display. |
| Pulsing red actuator marker and **Feedback lost** | The view previously received joint feedback for that actuator and the feedback has gone stale. It returns to blue when feedback resumes. |

If the model loads but the pose stays fixed, check the connection profile and find the project's joint feedback topic in [Topics](nodes-topics-services.md). Check whether the expected joint names appear and whether messages continue to arrive. If the model geometry and ROS transforms disagree, inspect the published frames in [TF Frames](tf-frames.md).
