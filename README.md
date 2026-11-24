# Robotics Ecosystem 2027

**Planned release · December 13, 2026**

Robotics Ecosystem 2027 is a local desktop workbench for ROS 2. Open a workspace, build and launch a robot or simulation, inspect the running system, and record or analyze ROS bags.

## See the robot and its ROS data together

- **[Holographic View](docs/holographic-view.md)** shows the robot model, sensor and actuator markers, and joint feedback in Live Kinematics.
- **[Split View and docking](docs/split-view-and-docking.md)** lets you place ROS panels side by side and dock a compatible running application such as Gazebo.
- **[Live Inspector](docs/live-inspector.md)** lets you monitor topic messages, plot numeric fields, and inspect odometry or laser scans.
- **[Offline Bag Analysis](docs/offline-bag-analysis.md)** lets you scrub a recording, step through messages, and compare signals on a shared timeline.

## Download and install

The Ubuntu installer is planned as a prebuilt **.deb**. Check [GitHub Releases](https://github.com/GibsonAB/robotics-ecosystem-2027/releases) for the installer, compatibility details, and the SHA-256 checksum when the release is published.

Start with [Installation](docs/installation.md), then follow [First run with a ROS 2 rover](docs/first-run.md).

## User guides

| Guide | What you can do |
| --- | --- |
| [Build & Launch](docs/build-and-launch.md) | Select a workspace, build it, run a launch file, and check output. |
| [Code & Packages](docs/code-and-packages.md) | Browse and edit project files, create ROS 2 packages, and rebuild. |
| [Tools & Supported Apps](docs/tools.md) | Choose an external tool and understand its prerequisites and launch workflow. |
| [Nodes, Topics & Services](docs/nodes-topics-services.md) | Discover nodes, echo and publish topics, and inspect service interfaces. |
| [TF Frames](docs/tf-frames.md) | Inspect the frame tree and look up transforms. |
| [ROS Bags](docs/ros-bags.md) | Record selected topics and replay them on the intended connection. |
| [ROS Controls](docs/ros-controls.md) | Inspect controller state, parameters, lifecycle nodes, actions, and components. |
| [Connections & Settings](docs/connections.md) | Set up ROS domain profiles, discovery, and desktop preferences. |
| [Troubleshooting](docs/troubleshooting.md) | Diagnose build, launch, discovery, visualization, and bag issues. |

These guides describe the pre-release workflow. The release notes will identify supported platform and external-tool combinations for the published installer.
