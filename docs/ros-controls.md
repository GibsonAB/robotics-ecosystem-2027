# ROS Controls

ROS Controls brings together interfaces that a running project exposes. Start with a simulator or a test system and check the active connection in the panel before making a change.

| Interface | How to read it |
| --- | --- |
| **Parameters** | Select a node and inspect its names, types, and values. Where editing is available, check the type, permitted range, and target node before applying a change. |
| **Lifecycle nodes** | Inspect the current state. Use only the transition offered for the intended node and verify the resulting state. |
| **Actions** | Inspect the action name and goal type. Where supported, monitor the goal status and result after sending a goal in simulation. |
| **Components** | Identify the intended component container and inspect the components it contains. |
| **ros2_control** | Find the controller manager, review available controllers and their states, and inspect hardware interfaces where shown. |

For a simulator check, launch a project that uses `ros2_control`, select its connection, locate its controller manager, and verify the expected controller state after launch. An empty controller list can indicate a mismatched ROS profile, a namespace difference, or a controller manager that failed to start. Check [Connections](connections.md) and the [launch output](build-and-launch.md).
