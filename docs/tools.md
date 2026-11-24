# Tools & Supported Apps

The Tools panel is for launching external applications installed on your machine. Check the release notes for the tested platform and executable combinations, and use your project's ROS and simulator setup instructions for its dependencies.

| Tool | What to check before opening it | What to do after it opens |
| --- | --- | --- |
| **RViz2** | Install RViz2 for the ROS distribution in use. Select the same connection as your robot or simulator when launching it. | Choose a fixed frame published by the project and add an appropriate display such as TF, RobotModel, or LaserScan. |
| **rqt** | Install rqt and any plugins needed for your workflow. | Select the desired plugin. For graph inspection, use the graph plugin with a running ROS system on the same connection. |
| **Gazebo** | Install the simulator generation and ROS integration required by your project. Check the launch instructions for the matching bridge, models, and plugins. | Open a world or use the project's launch file to start the simulation with its ROS nodes. Verify that the project's expected ROS topics appear. |

To open a supported app, find it in **Tools** and use its launch action. Read the tool output if the process exits or no window appears. Launching a general tool is useful for inspecting a session. Use [Build & Launch](build-and-launch.md) when the project needs to start several processes together.

Gazebo Harmonic docking was exercised in a development build under X11/XWayland. See [Split View and docking](split-view-and-docking.md) for the workflow. Isaac Sim launch and detection are pending verification for the public release.
