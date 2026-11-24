# Troubleshooting

| Symptom | First checks |
| --- | --- |
| Installer reports a dependency problem | Compare Ubuntu version and CPU architecture with the release notes. Recheck the installer filename and checksum. |
| Build fails | Confirm the workspace root and ROS distribution. Read the first package error and check the project's dependency instructions. |
| Launch exits or no simulator opens | Read the full launch output. Confirm the chosen file starts the simulator and the requested Gazebo version and plugins are installed. |
| Nodes or topics are missing | Match the selected profile with the launch domain and discovery mode. Verify the project has started and check its namespace. |
| Topic appears but Echo is blank | Check simulator pause, the publisher or bridge, and compatible subscriber QoS. |
| Holographic View shows a static pose | Confirm model selection and joint feedback on the active profile. Review [Holographic View](holographic-view.md) for the feedback indicator. |
| An external window won't dock | Confirm the external app is running and check the supported display session. See [Docking](split-view-and-docking.md#dock-an-external-window). |
| TF lookup fails | Check exact frame names, a connected tree, and current transforms on the intended profile. |
| Bag displays no messages on replay | Check that the recorder finalized, that the bag contains the expected topics, and that the viewer uses the playback connection. |

When reporting a problem, include the Robotics Ecosystem 2027 version, Ubuntu and ROS 2 versions, the tool or simulator version if relevant, the smallest set of steps that reproduces it, and the relevant output. Remove credentials, private project details, and private paths before posting public logs.
