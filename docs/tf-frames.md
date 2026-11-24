# TF Frames

TF describes how coordinate frames are positioned and oriented relative to one another. A typical rover might publish a moving `odom → base_link` transform and a fixed `base_link → laser` transform.

1. Open **TF** on the same connection as the rover and locate `base_link`.
2. Expand its children and find the LiDAR frame. Select it and inspect the parent, translation, rotation, and timestamp where shown.
3. Use the transform lookup with `base_link` as the target and `laser` as the source to inspect the pose of the laser frame expressed in the base frame.
4. Check frame connectivity if the lookup fails. Confirm the exact frame names and whether the project is publishing to `/tf` and `/tf_static`.
5. For a dynamic transform that stops updating, verify that the simulator is running and the relevant publisher is alive. Static transforms are expected to remain unchanged.

Use frame search, zoom, and graph export where available when the tree is large. Per-transform publisher attribution may be unavailable on Humble. Use [Nodes, Topics & Services](nodes-topics-services.md) to investigate discovered publishers separately.
