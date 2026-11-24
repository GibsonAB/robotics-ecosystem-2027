# Robotics Ecosystem 2027

**Planned release · December 13, 2027**

Robotics Ecosystem 2027 is a local desktop workbench for ROS 2. Open a workspace, build and launch a robot or simulation, inspect the running system, and record or analyze ROS bags.

## Download and install

The Ubuntu installer is planned as a prebuilt **.deb**. Check [GitHub Releases](https://github.com/GibsonAB/robotics-ecosystem-2027/releases) for the installer, compatibility details, and the SHA-256 checksum when the release is published.

Start with [Installation](docs/installation.md), then follow [First run with a ROS 2 rover](docs/first-run.md).

## Features

| Feature | What you can do |
| --- | --- |
| [Holographic View](docs/holographic-view.md) | Inspect the robot model, locate sensors and actuators, and follow live joint feedback. |
| [Split View & Docking](docs/split-view-and-docking.md) | Arrange workbench panels side by side and dock a compatible external window such as Gazebo. |
| [Live Inspector](docs/live-inspector.md) | Monitor live messages, plot numeric fields, and inspect odometry or laser scans. |
| [ROS Bags](docs/ros-bags.md) | Record and replay ROS topics, then inspect saved messages and compare signals on a timeline with [Offline Bag Analysis](docs/offline-bag-analysis.md). |
| [Build & Launch](docs/build-and-launch.md) | Select a workspace, build it, run a launch file, and check output. |
| [Code & Packages](docs/code-and-packages.md) | Browse and edit project files, create ROS 2 packages, and rebuild. |
| [Tools & Supported Apps](docs/tools.md) | Choose an external tool and understand its prerequisites and launch workflow. |
| [Nodes, Topics & Services](docs/nodes-topics-services.md) | Discover nodes, echo and publish topics, and inspect service interfaces. |
| [TF Frames](docs/tf-frames.md) | Inspect the frame tree and look up transforms. |
| [ROS Controls](docs/ros-controls.md) | Inspect controller state, parameters, lifecycle nodes, actions, and components. |
| [Connections & Settings](docs/connections.md) | Set up ROS domain profiles, discovery, and desktop preferences. |

For help with build, launch, discovery, visualization, or bag issues, see [Troubleshooting](docs/troubleshooting.md).

These guides describe the pre-release workflow. The release notes will identify supported platform and external-tool combinations for the published installer.
