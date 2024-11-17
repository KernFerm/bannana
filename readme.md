# Bubbles The Dev Youtube To MP3 Downloader

This Python script downloads audio from a YouTube video URL or playlist and converts it to MP3 files at 192 kbps. It utilizes the `yt-dlp` library for downloading, `pydub` for audio conversion, and `mutagen` for embedding metadata.

## Features

- Downloads audio from a YouTube video or playlist.
- Converts the audio to MP3 files with a bitrate of 192 kbps.
- Embeds metadata (title, artist, album) into the MP3 files.
- Automatically checks if `ffmpeg` is installed and configures its path for `pydub`.
- Cleans up temporary files after conversion.

## Requirements

- **Python** 3.11 [Python 3.11.6 Installer](https://github.com/KernFerm/Py3.11.6installer)
- **ffmpeg** (must be installed and added to PATH)
- **Python packages**:
  - `yt-dlp`
  - `pydub`
  - `mutagen`

## Discord

If you have any issues, join our [Discord](https://www.discord.fnbubbles420.org/invite) - Fnbubbles420 Org Community.  
- Head to the channel `free-music`
- Ping `Bubbles` for support.

### Project Link
- [Pre-Release](https://github.com/KernFerm/Bubbles_The_Dev_Youtube_To_MP3/releases/tag/youtube-to-mp3)

---

## Installation

### 1. Install ffmpeg

#### Option A: Install with `winget` (Recommended for Windows Users)

Run this command in **Command Prompt** or **PowerShell** as Administrator:

```
winget install --id Gyan.FFmpeg -e --source winget
```

#### Option B: Download and Manually Install

1. Download the latest `ffmpeg` build from [ffmpeg.org](https://ffmpeg.org/download.html) or [gyan.dev](https://www.gyan.dev/ffmpeg/builds/).
2. Extract the files and add the `bin` directory (e.g., `C:\ffmpeg\bin`) to your system PATH.

- Verify `ffmpeg` installation by running:

```
ffmpeg -version
```

### 2. Install Python Packages

Install the required packages by running:

```
pip install yt-dlp pydub mutagen
```

---

## Usage

1. Clone or download this repository.

### 📥 How to Download the Repo (First-Time Users)

Click the link to read [**Instructions**](https://www.gitprojects.fnbubbles420.org/how-to-download-repos) 📄.

2. Run the script:

```
python main.py
```

3. Choose whether to download a single track or a playlist:
   - Enter `track` or `playlist` when prompted.

4. Enter the YouTube URL when prompted.

---

## Example

```
$ python main.py FFmpeg found at: C:\path\to\ffmpeg.exe Do you want to download a single track or a playlist? 
(Enter 'track' or 'playlist'): playlist 
Enter the YouTube URL: https://www.youtube.com/playlist?list=example Downloading and converting audio... 
Processing metadata for Track Title... 
Download and conversion completed! 
MP3 files saved in: downloaded_audio/
```


---

## How-To Video
new vid coming soon...
![pic]()

---

## Troubleshooting

- **FFmpeg Not Found**: If you see the message `FFmpeg is not installed or not found in PATH`, please ensure that `ffmpeg` is installed and correctly added to your PATH.
- **Metadata Not Embedded**: Ensure the `.info.json` files are being generated by `yt-dlp` and the script has write access to the output directory.

---

## Notes

- Ensure `ffmpeg` is installed and added to your system PATH so `pydub` can locate it.
- If installed with `winget`, `ffmpeg` may be located at `C:\Users\<username>\AppData\Local\Microsoft\WinGet\Links`.

---

## LICENSE

- **This project is proprietary, and all rights are reserved by the author.**
- **Unauthorized copying, distribution, or modification of this project is strictly prohibited.**
- **You must have written permission from the developer or the FNBUBBLES420 ORG to use or distribute this project.**

---
---
