# Nodes, Topics & Services

Select the connection running your robot or simulation before using these panels.

- **Nodes** shows discovered ROS processes by their node names. Look for the names and namespaces expected by your project.
- **Topics** lists named message streams and their types. Echo subscribes and displays messages. Publish sends a message to the chosen topic.
- **Services** lists request/response endpoints. Inspect the service type and request fields before using any call action in the released UI.

## Check a simulated LiDAR

1. Start the rover simulation and open **Topics**.
2. Find `/scan`, or the mapped scan topic for your project. Confirm its type is `sensor_msgs/msg/LaserScan`.
3. Start **Echo** and look for repeating messages. If the topic is listed with no samples, check whether the simulator is paused, the bridge is running, or the echo QoS is incompatible.

## Publish a test message

Use a local simulation or isolated test connection. For example, with a test subscriber on `/ecosystem_demo/chatter` that expects `std_msgs/msg/String`, select that topic and type and set the `data` field to `hello`. Confirm receipt in the subscriber. Inspect the topic name, type, and connection before sending. See [Live Inspector](live-inspector.md) when you need charts or recent history.
