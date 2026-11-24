# Offline Bag Analysis

Offline Bag Analysis lets you examine recorded messages on a shared timeline. Start with a bag containing `/cmd_vel`, `/odom`, and `/scan` if your project publishes all three. Use any available subset to follow the corresponding steps.

1. Open an existing bag in the bag analysis view. Check its duration and topic list.
2. Add a numeric plot for commanded forward velocity from `/cmd_vel`. Add odometry velocity from `/odom` and use the shared time cursor to compare them.
3. Open the XY odometry view and the LiDAR snapshot if those topics are present. Move the playhead and check how the views update.
4. Inspect a raw message to see the decoded fields and timestamp. Use the step controls to walk through consecutive messages, including messages that share a timestamp.
5. When a plotted sample precedes the selected playhead, check its sample age before interpreting the values as simultaneous.

See the release notes for the verified bag formats and compression support. The development audit exercised split SQLite bag decoding and plots. For playback that publishes messages to ROS 2, use [Replay to ROS](ros-bags.md#replay-to-ros).
