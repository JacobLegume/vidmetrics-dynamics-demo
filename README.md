
# 📊 vidmetrics-dynamics-demo

![Repository logo](/img/bg.jpg)
A simple demo that compares video quality (PSNR/SSIM) across various codecs, bitrates, and levels of motion to study how compression affects dynamic scenes.  

*Great for anyone who wants to get started with video quality evaluation.*

# WORK IN PROGRESS
## Description


`vidmetrics-dynamics-demo` is an approachable project that demonstrates how video compression affects perceived quality using objective metrics such as **PSNR** and **SSIM**, with a focus on **scene dynamics** (amount of motion), **codecs**, **bitrates**, and **resolutions**.

This project is ideal for anyone interested in video quality evaluation, media encoding, or understanding how different codecs impact video quality, especially in dynamic scenes.
        


### What is going to happen?

1.  The project begins with **2 original source video files** containing varying levels of motion.
    
2.  It processes these files and generates **50 output files** with the following parameters:
    
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
```bash
ffmpeg version 2025-03-31-git-35c091f4b7-full_build-www.gyan.dev Copyright (c) 2000-2025 the FFmpeg developers
built with gcc 14.2.0 (Rev1, Built by MSYS2 project)
```

![Win - verify](/img/win3.gif)

---
#### macOS


---
#### Linux (Ubuntu/Debian)

## Installation*

To get this repository on your computer:

1. **Install Git (if not installed)**

If you don't have Git installed, you can download and install it from [Git's official website](https://git-scm.com/downloads).

2. **Clone the repository:**

Open your command prompt and run the following command to clone the repository to your local machine:

```bash
git clone https://github.com/JacobLegume/vidmetrics-dynamics-demo
```

#### Download Video Sources
The project is based on videos from [ultravideo.fi](https://ultravideo.fi/dataset.html). If you want to follow along:

1. Go to the [UVG dataset page](https://ultravideo.fi/dataset.html) and choose a video.
2. Take note of its details (length, frame rate).
3. Download any version in **YUV RAW format**, e.g. 3840×2160 8-bit YUV RAW.
4. Unzip the file into the cloned repository directory.

#### Disclaimer and Attribution

This project uses example video content from external sources for demonstration and evaluation purposes only.  The original video files are **not included in this repository**.

Specifically, the demonstration uses videos from [ultravideo.fi](https://ultravideo.fi/dataset.html), which are licensed under [Creative Commons BY-NC 3.0](https://creativecommons.org/licenses/by-nc/3.0/). These materials are intended **only for non-commercial and educational use** in accordance with their license.

If you use these videos in your own work, please cite the original authors:

*A. Mercat, M. Viitanen, and J. Vanne, “[UVG dataset: 50/120fps 4K sequences for video codec analysis and development,](https://dl.acm.org/doi/abs/10.1145/3339825.3394937)” *Proc. ACM Multimedia Systems Conference (MMSys)*, Istanbul, Turkey, June 2020. [Tuni.fi](https://researchportal.tuni.fi/en/publications/uvg-dataset-50120fps-4k-sequences-for-video-codec-analysis-and-de) | [PDF](https://cris.tuni.fi/ws/portalfiles/portal/42239069/MMSys20_UVG_Dataset_Camera_ready.pdf)*

The source code of this project is licensed under the MIT License and does not include any copyrighted
video data.

---

## Usage Example*

**placeholder for an actual usage example**

**placeholder for an actual usage example**

**placeholder for an actual usage example**

**placeholder for an actual usage example**

---

## Project Structure*

```bash
git-tutorial/
├── README.md
├── LICENSE
└── img/
    └── bg.jpg
```


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- Jakub Warzych - Main Author - [JacobLegume](https://github.com/JacobLegume)

## Contributing

Feel free to fork this repository, open issues, and submit pull requests. All contributions are welcome!
