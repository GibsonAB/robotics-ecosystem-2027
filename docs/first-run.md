# First run with a ROS 2 rover

Use a ROS 2 rover workspace you can already build for your ROS distribution. For this example, choose one with a simulator launch file, a LaserScan topic, and TF from the robot base to its LiDAR. The examples use `/scan`, `base_link`, and `laser`. Substitute your project's names where they differ.

1. **Connect.** Open Settings and choose a profile for a local simulation. Use the same domain for tools that need to see your simulation. See [Connections & Settings](connections.md).
2. **Build.** Open **Code**, select the workspace folder, and build it. Check the output before launching. See [Build & Launch](build-and-launch.md).
3. **Launch.** Choose the project's simulator launch file. Wait for the simulator and the project's ROS processes to start. Read the launch output if either is missing.
4. **Inspect.** Find the project processes in **Nodes**. Open **Topics** and echo `/scan`. Confirm that messages arrive while the simulation runs. See [Nodes, Topics & Services](nodes-topics-services.md).
5. **Check TF.** Find the base and LiDAR frames, then look up the transform between them. See [TF Frames](tf-frames.md).
6. **Record.** Record `/scan` for about ten seconds. Stop recording and wait for the bag to finalize. See [ROS Bags](ros-bags.md).
7. **Analyze and replay.** Open the bag in [Offline Bag Analysis](offline-bag-analysis.md) and scrub to a laser scan. To test replay, first stop the simulation or use a separate test domain so you can distinguish playback messages from live messages. Echo the recorded topic on the replay connection.

For a second pass, open [Holographic View](holographic-view.md) and [Live Inspector](live-inspector.md) side by side using [Split View](split-view-and-docking.md).
