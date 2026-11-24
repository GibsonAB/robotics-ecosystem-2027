# Split View and docking

Split View places multiple workbench panels in the same window. Docking brings a compatible external application window into a pane.

## Arrange workbench panels

1. Open the first panel, such as **Holographic View**.
2. Right-click a second item in the sidebar and choose **Open to the Right** or **Open Below**. You can also start from the top-bar **Split View** control.
3. Drag the divider to resize the panes. Use the pane's close button to remove it from the layout.

Try Holographic View beside [Live Inspector](live-inspector.md). Watch the model while plotting a field from a topic on the same connection.

## Dock an external window

1. Start the external app using [Tools](tools.md) or its usual launcher.
2. Open Split View and use the pane's docking controls to select the running window.
3. Resize the pane and confirm that the external app redraws inside it.
4. Use the undock action to return it to its own window. Undocking does not end the application session.

The 4.0.50-1 development check exercised docking, resizing, pausing, and undocking with **Gazebo Harmonic** under X11/XWayland. Native Wayland docking and compatibility with other applications still need release verification. If a window does not dock, use it as a separate window and check the release notes for the supported display session. Split View can also open web links in a pane.
