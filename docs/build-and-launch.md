# Build & Launch

## Select and build a workspace

1. Open **Code** and select the workspace folder. For a typical colcon workspace, choose the root containing `src/`.
2. Check the active workspace in Code. If you registered several folders, switch to the one containing the package you intend to run.
3. Install any prerequisites specified by the project. Choose **Build Workspace**, then read the output in **Launch**. Resolve the first compiler or dependency error before retrying.

## Run a launch file

1. Select the project launch file in **Launch**, or use the launch action on the file in the Code tree when available.
2. Select the intended [connection profile](connections.md).
3. If the project documents launch arguments, supply them using the names and values that the launch file expects. Check any simulator or visualization flags before starting.
4. Start the launch and read its output. Check [Nodes and Topics](nodes-topics-services.md) to confirm that outputs are appearing on the selected connection.
5. To stop the app-managed launch, use its **Stop** action and check the session output for shutdown.

For a rover demonstration, choose the launch intended to start the simulator. An RViz-only launch can show the robot and its frames while a separate simulator is responsible for physics and simulated sensors. Use the project's launch-file documentation to identify what each launch starts.
