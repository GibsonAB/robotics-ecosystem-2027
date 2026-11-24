# Live Inspector

Live Inspector lets you follow incoming ROS 2 data, chart numeric fields, and see how the stream changes while a system is running.

1. Select the connection used by the robot or simulator.
2. Open **Live Inspector**. Add a discovered topic and check the message type and last update.
3. Select a numeric field. For a rover publishing `nav_msgs/msg/Odometry` on `/odom`, try the forward velocity field `twist.twist.linear.x`.
4. If your project publishes `/scan`, use the laser view to inspect a scan in its sensor frame. The odometry view can show a trail and heading for an odometry topic.
5. Pause the displayed timeline to inspect recent history. Incoming data continues to populate the history. Scrub back, then choose **Go Live** to return to the newest samples.

Use rate to see how often messages are arriving and age to see how old the current displayed sample is. For a blank plot, check that the topic has traffic, the field is numeric, and the correct connection is selected. Treat plotted sensor previews as previews and consult the raw message when you need the full input.

Use [Offline Bag Analysis](offline-bag-analysis.md) to do the same kind of investigation on a saved recording.
