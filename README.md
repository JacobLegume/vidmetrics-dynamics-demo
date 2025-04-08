
# 📊 vidmetrics-dynamics-demo

![Repository logo](/img/bg.jpg)
A simple demo that compares video quality (PSNR/SSIM) across various codecs, bitrates, and levels of motion to study how compression affects dynamic scenes.  

*Great for anyone who wants to get started with video quality evaluation.*

## Description


`vidmetrics-dynamics-demo` is an approachable project that demonstrates how video compression affects perceived quality using objective metrics such as **PSNR** and **SSIM**, with a focus on **scene dynamics** (amount of motion), **codecs**, **bitrates**, and **resolutions**.

This project is ideal for anyone interested in video quality evaluation, media encoding, or understanding how different codecs impact video quality, especially in dynamic scenes.


### Key Features

-   Explanation of key concepts such as:
    
    -   **Raw YUV format**
        
    -   **H.264 / H.265 / VP9 codecs**
        
    -   **Bitrate** and its effect on video quality
        
-   A full set of commands used in the processing pipeline:
    
    -   All **FFmpeg** commands included
        
    -   Each step explained with comments and usage examples
        


### What is going to happen?

1.  The project begins with **2 original source video files** containing varying levels of motion.
    
2.  It processes these files and generates **48 output files** with the following parameters:
    
    -   **3 codecs**: H.264, H.265, VP9
        
    -   **8 bitrates**: 100 kbps, 500 kbps, 1000 kbps, 2000 kbps, 3000 kbps, 4000 kbps, 5000 kbps, 6000 kbps
        
    -   **2 resolutions**: 720p and 1080p
        
    -   Plus **reference (uncompressed)** files for comparison
        
3.  The output files are compared against the source files using:
    
    -   **PSNR** (Peak Signal-to-Noise Ratio)
        
    -   **SSIM** (Structural Similarity Index)
        
4.  The results are aggregated and analyzed to:
    
    -   Compare quality degradation across different codecs, bitrates, and resolutions
        
    -   Draw conclusions about which settings perform best in specific scenarios

## Prerequisites*
### FFmpeg 
#### Windows
**Download**
1. Go to the [FFmpeg Download page](https://ffmpeg.org/download.html).
2. Choose Windows and click the "Windows builds from gyan.dev"
3. Download the appropriate version. If you don't know which one is right for you, it's usually `ffmpeg-git-full.7z`
4. Extract the ZIP file somewhere, for example `C:\ffmpeg`

![Win - which to download](/img/win1.gif)

**Add to PATH**
1. Open the Control Panel → System → Advanced system settings → Environment Variables.

![Win - add to path](/img/win2.gif)

**Verify**
1. Open **Command Prompt**
2. type:
```bash
ffmpeg -version
```
3. If everything is correctly installed, you should see FFmpeg version information.

![Win - verify](/img/win3.gif)

---
#### macOS


---
#### Linux (Ubuntu/Debian)

## Installation*


## Usage Example*


## Project Structure*

```bash
git-tutorial/
├── README.md
├── LICENSE
└── img/
```


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- Jakub W. - Main Author - [JacobLegume](https://github.com/JacobLegume)

## Contributing

Feel free to fork this repository, open issues, and submit pull requests. All contributions are welcome!
