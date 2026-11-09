# Concord CAM

Concord CAM is a standalone macOS app for preparing CNC jobs, simulating material removal, and connecting to a Makera Z1 on your local network.

## Download

Download the macOS preview ZIP from [Releases](https://github.com/kixel-cz/concord-cam/releases).

The preview targets **macOS 14 or later on Apple Silicon**. Unzip the download, move **Concord CAM.app** to Applications, and open it from Finder.

To check the installed version and build number, choose **Concord CAM → About Concord CAM** in version 0.1.2 or later.

## First job

1. Create a project or open a saved `.cam` file. Keep its model or drawing files beside it when moving a project between computers.
2. Import your model from the **Project** menu. For a milling job, set up the stock, choose a material, and add your cutter under **Tools → Library**.
3. Generate the toolpath and play the material-removal simulation. Use **Project → Export G-code** to save the verified program for offline use.
4. To connect to a Z1, put the Mac and the machine on the same local network. Open **Machine**, select the controller or enter its IP address, and click **Connect**. Allow local network access if macOS prompts you.

## Feedback

Report problems in [Issues](https://github.com/kixel-cz/concord-cam/issues). Include the Concord CAM version, your macOS version, and the steps to reproduce the issue. For connection problems, also include the controller model and firmware version if known.

## Development

The macOS app shares its CAM engine, project format, and user interface with ConcordOS. Release notes identify the ConcordOS source commit used for each build. The app icon is the ConcordOS emblem on the system's dark tile with the app name set below it.