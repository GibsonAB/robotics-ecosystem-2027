# Code & Packages

Open **Code**, select a workspace, and open a file in the editor. The tree is useful for checking a package's `package.xml`, source files, launch files, and configuration together.

## Edit and run a change

1. Open a Python node you control and change an existing log message.
2. Save the file. Build the selected workspace and check the output.
3. Stop the previous run, relaunch the node using the same project launch, and check that the new message appears.

## Create a package

Open the package creation action in Code, choose Python or C++, give the package a unique valid ROS name, and review the files it generates. Add dependencies and executable or entry-point configuration as required by your package. Build the workspace and resolve any errors before launching the new node. Package and support-file templates can vary with the release.

File-tree changes affect the selected workspace on disk. Verify the active workspace and file path before renaming or deleting a file or package. See [Build & Launch](build-and-launch.md) for the build and session workflow.
