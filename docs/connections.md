# Connections & Settings

A connection profile identifies the ROS environment a panel or launch uses. ROS processes need a compatible discovery configuration and the same ROS domain to see each other directly.

## Create and use a profile

1. Open **Settings** and find the ROS connection profiles.
2. Name the profile and choose its domain ID. For a same-machine simulation, choose localhost discovery if all participating processes are local. For a robot on the network, use its domain and compatible network discovery settings.
3. Select the profile before launching a project. Check the active connection in the panel you use to inspect nodes, topics, TF, and bags.
4. When switching from a simulator to a robot or another workspace, recheck the connection before publishing, replaying, or changing a controller.

For example, you might use **Local Rover** on domain 15 for simulation and **Lab Robot** on domain 14 for network discovery. Those IDs are examples. Use the values actually configured on your system.

Settings also provides desktop preferences such as themes. The sidebar can be hidden to make room for [Split View](split-view-and-docking.md).

## Vitals

If Vitals is available in your build, check its active ROS profile before comparing observations across systems. Use [Nodes, Topics & Services](nodes-topics-services.md) to confirm graph discovery and [Live Inspector](live-inspector.md) to check message arrival and age directly. Consult the release notes for the metrics verified for the installer.
