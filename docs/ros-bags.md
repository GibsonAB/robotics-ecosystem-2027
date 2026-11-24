# ROS Bags

Use ROS Bags to capture ROS messages during a live session and replay them later. Check the [connection profile](connections.md) before starting either operation.

## Record a ten-second sample

1. With the rover simulator running, open **Bags** and select its connection.
2. Select `/scan` or the mapped scan topic. To compare motion with sensor data, also select `/odom` if available.
3. Set the recording destination and start recording. Wait about ten seconds, then stop and allow the recorder to finalize the bag.
4. Check its path, topic list, and message counts. Open [Offline Bag Analysis](offline-bag-analysis.md) to review the data.

## Replay to ROS

1. Open the saved bag and check its topics before playback.
2. Select the intended playback connection. For a first test, use a local test domain or stop the simulator so live messages do not overlap with replay.
3. Start **Replay to ROS**. Echo a recorded topic on that connection and confirm that messages arrive.
4. Stop playback and check the session status when done.

A bag can contain command topics as well as sensor data. Review the recorded topics and playback destination before replaying on a robot network.
