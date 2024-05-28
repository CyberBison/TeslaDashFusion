# TeslaDashFusion

Welcome to TeslaDashFusion, the ultimate tool for Tesla vehicle owners who wish to effortlessly merge and manage their dashcam footage. Whether you're looking to create comprehensive video compilations from your Tesla's multiple cameras or simply organize your recordings, TeslaDashFusion is here to simplify the process.

## Getting Started with TeslaDashFusion

### Installation Options

Installing TeslaDashFusion is straightforward, with two primary methods available:

- **Installer Download**: Grab the installer specifically tailored for your operating system to enjoy a hassle-free setup process.
  
- **Manual Build**: For those who prefer a more hands-on approach or need a custom build, TeslaDashFusion can be compiled from the source using Node.js and npm.

### How to Use TeslaDashFusion

TeslaDashFusion is designed for simplicity and efficiency. To get started, follow these easy steps:

1. **Source Folder Selection**: Begin by choosing a source folder. This directory should contain subfolders corresponding to the four camera feeds from your Tesla, each filled with videos bearing their original filenames as generated by the car. For instance, you might select something like `F:\TESLADRIVE\TeslaCam\SavedEntries\`.

2. **Destination Folder Selection**: Decide where you'd like the fused videos to be stored. TeslaDashFusion will organize the processed footage into subfolders mirroring the original structure. Each video will also be tagged with a layout identifier, such as "_layout1", "_layout2", etc., for easy identification.

3. **Layout Selection**: Pick one or more video layouts according to your preferences for the final video composition.

4. **Concurrent Processing**: Set the number of folders you wish to process simultaneously. This allows for efficient video processing tailored to your system's capabilities.

### Building TeslaDashFusion Yourself

For enthusiasts interested in compiling TeslaDashFusion on their own, the process is as follows:

1. **Preparation**: Ensure that you have all necessary dependencies for Electron and Electron Builder installed on your system. This step is crucial for a successful build.

2. **Cross-Platform Builds**: If you're aiming to build a Windows version from a non-Windows environment (e.g., Linux or WSL 2), begin by running `npm install` on a Windows machine. This step is necessary to procure the correct `ffmpeg-static` dependencies for the target platform.

3. **Build**: Once you've installed the required node, simply build for your system using one of the following command:

- For Linux: `npm run dist-lin`
- For Windows: `npm run dist-win`
- For MacOS: `npm run dist-mac`

4. **Run**: The executable will be created under the `dist` folder

## Conclusion

TeslaDashFusion brings a new level of convenience and control to managing your Tesla's dashcam footage. With its user-friendly interface and powerful features, it's the perfect companion for any Tesla owner looking to enhance their video compilation efforts. Whether you choose to download the ready-made installer or build the application yourself, TeslaDashFusion is ready to meet your needs.

## Licensing

TeslaDashFusion is released under the GNU General Public License version 3 (GPL-3.0). This license ensures that the software remains free and open source, allowing users to view, modify, and distribute the code.

### Use of FFmpeg

TeslaDashFusion utilizes FFmpeg, a powerful multimedia framework, for video processing and manipulation. FFmpeg is licensed under the GNU Lesser General Public License version 2.1 (LGPL-2.1) or later. This means that TeslaDashFusion is able to incorporate and distribute FFmpeg as part of its functionality.

It's important to note that FFmpeg has its own licensing terms and conditions. When using TeslaDashFusion, you are also bound by the terms of the FFmpeg license. Make sure to review and comply with the FFmpeg licensing requirements when using TeslaDashFusion.

For more information about the GNU GPL-3.0 license, visit the [GNU website](https://www.gnu.org/licenses/gpl-3.0.en.html). To learn more about FFmpeg and its licensing, visit the [FFmpeg website](https://www.ffmpeg.org/legal.html).

## Disclosure

TeslaDashFusion is not affiliated with Tesla, Inc. It is an independent software tool developed by a third-party developer.

## Known bugs

- (BUG) Quitting the app can throw an unexpected error

## ToDo / Roadmap

Here's a short list of upcoming features or features that would be nice to have:

- Example of layouts to help user chose the right layout
- Overall GUI improvement
- Showing a global progression instead of the console output, by example: "Processing subfolder 5 of 150"
- Add an option to show the timestamp on the video and other info from `content.json` created by the Tesla dashcam
- Create a cool app icon