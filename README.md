# Project: Volumetric Video Loader

## Overview

This project allows users to load and visualize PLY files efficiently in Unity. It supports real-time playback, video recording, and folder browsing for an enhanced user experience.

## Features

- **PLY File Import**: Load 3D models from PLY files.
- **Playback Control**: Slider to navigate through frames.
- **Video Recording**: Record the rendered sequence and save it as a video.
- **Lighting Control**:
  - **Ambient Lighting**: Adjust overall scene brightness.
  - **Directional Light**: Control light intensity and position.
  - **Point Light**: Position and intensity control for focused illumination.
- **Frame Rate Control**: Adjust the playback speed.
- **Point Cloud Size Control**: Modify the size of point cloud elements for better visualization.
- **Object Manipulation**:
  - Reset object position.
  - Rotate object using the mouse to highlight light effects using normals.
- **Animation Control**:
  - **Play Animation**: Start the sequence playback.
  - **Stop Animation**: Pause the playback.
- **Keyboard Shortcuts**:
  - `Space`: Start/Stop video recording.
  - `Slider`: Navigate frames.
- **Folder Selection**: Browse folders via a FolderPicker

## How to Use (Standalone .exe)

### **Installation**

1. Download the latest `.zip` file from the release section.
2. Extract the contents to a folder of your choice.

### **Running the Application**

1. Open the extracted folder.
2. Open a terminal in the extracted folder. 
3. run the command "python -m http.server" to run the http server
4. launch a browser of your choice. 
4. run the localhost http://localhost:8000/

### **FFMPEG use**
1. To record properly the video. You should install ffmpeg and change its exe path in the script DynamicUIManager in the ConvertToVideo function.
2. You should also change the video output path in the Start method of the DynamicUIManager script to match your needs

### **Using the Application**

1. Click **Browse Folder** to select the directory containing your PLY files.
2. Use the **slider** to navigate through the sequence.
3. Adjust lighting settings for ambient, directional, and point lights.
4. Modify **frame rate** and **point cloud size** for better visualization.
5. Use the **mouse** to rotate the object and observe light effects.
6. Click **Reset Position** to restore the object’s default position.
7. Click **Play Animation** to start the sequence playback.
8. Click **Stop Animation** to pause the sequence.
9. Click **Start Recording** to record the sequence as a video.
10. Press `Space` to stop recording.
11. The video will be saved in a directory named Recorded video and the name will be output.mp4.

## Known Issues

- **WebGL Folder Selection**: Requires JavaScript integration; may not work in all browsers.
- **Large Files**: Some large PLY files might take longer to load, even with GPU acceleration.

## Future Improvements

- **GPU Acceleration**: Faster processing using Compute Shaders.
- **Web version**: web version is in progress
- Add support for more 3D formats (OBJ, STL, etc.).
- Improve rendering performance for larger datasets.
- Implement advanced lighting effects and shadows.


