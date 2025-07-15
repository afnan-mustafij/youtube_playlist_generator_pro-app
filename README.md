# YouTube Playlist Generator Pro 🎥

**Generate YouTube playlist URLs from video links with style and ease!**

This Python-based GUI app transforms YouTube video URLs into playlist URLs for a channel’s full video library or uploads (including/excluding Shorts). Packed with video previews, duration estimates, and robust error handling, it’s perfect for content creators, researchers, or anyone who loves YouTube playlists. Run it as a script or build a standalone `.exe` for ultimate portability!

![App Screenshot](screenshot.png)  
*Compact UI with video previews, settings menu, and dark mode.*

## Features 🔥
- **Playlist Generation**: Convert YouTube video URLs to playlist URLs (full channel or uploads only).
- **Video Previews**: Display thumbnails, titles, channels, and durations for input URLs.
- **Duration Estimates**: Calculate total playlist duration using the YouTube API.
- **Batch Processing**: Handle multiple URLs in one go.
- **Video Count Filters**: Set min/max video counts with optional strict filtering.
- **Secure API Key**: Store your YouTube API key in a masked settings dialog.
- **Dark Mode**: Toggle between light and dark themes for a sleek look.
- **Export Options**: Copy playlist URLs to clipboard or export to CSV.
- **Cross-Platform Storage**: Config and logs saved in `AppData/Roaming` (Windows), `~/Library/Application Support` (macOS), or `~/.config` (Linux).
- **Robust Error Handling**: Fallback to web scraping if API fails, with detailed logs.
- **No History**: Clean slate every run, as you like it.

## Installation 🛠️

### Prerequisites
- Python 3.6+
- Required packages:
  ```bash
  pip install requests google-api-python-client tenacity pyperclip Pillow isodate appdirs
  ```

### Clone the Repo
```bash
git clone https://github.com/yourusername/youtube-playlist-generator.git
cd youtube-playlist-generator
```

### Optional: YouTube API Key
For video previews and duration estimates:
1. Get a YouTube Data API key from [Google Cloud Console](https://console.cloud.google.com/).
2. Enter it in the app’s Settings menu (securely masked).

## Usage 🚀
1. **Run the Script**:
   ```bash
   python youtube_playlist_generator_pro.py
   ```

2. **Enter URLs**:
   - Paste YouTube video URLs (one per line, e.g., `https://www.youtube.com/watch?v=7r0CHuqRkI8`) in the text area.
   - See real-time video previews with thumbnails and metadata.

3. **Configure Settings**:
   - Go to **Settings > Configure Settings** in the menu bar.
   - Set:
     - YouTube API key (optional, masked for security).
     - Include YouTube Shorts (default: off).
     - Dark Mode (default: off).
     - Request Timeout (5–30 seconds).
     - Min/Max Playlist Videos (1–1000/10000).
     - Enforce Video Count Filters (strict mode).
   - Save settings (stored in `AppData/Roaming/YouTubePlaylistGenerator/yt_playlist_config.json` on Windows).

4. **Generate Playlists**:
   - Click **Generate Playlists** to process URLs.
   - Playlists open in your browser.
   - View progress, logs, and duration estimates in the app.

5. **Manage Output**:
   - **Copy URLs**: Copy generated playlist URLs to clipboard.
   - **Export URLs**: Save to a CSV file.
   - **Clear Input**: Reset URLs and previews via **File > Clear Input**.

6. **Logs**:
   - Errors and logs are saved to `AppData/Roaming/YouTubePlaylistGenerator/yt_playlist_errors.log`.

## Building a Standalone `.exe` 💿
Turn the app into a portable Windows executable with a custom icon.

### Prerequisites
- Install PyInstaller:
  ```bash
  pip install pyinstaller
  ```

### Steps
1. **Get the Icon**:
   - Download or create `app_icon.ico` (256x256, red play button with playlist stack).
   - Place it in the same directory as `youtube_playlist_generator_pro.py`.
   - *Tip*: Use [icoconvert.com](https://icoconvert.com/) to convert a PNG to `.ico`.

2. **Build the `.exe`**:
   ```bash
   pyinstaller --onefile --windowed --icon=app_icon.ico youtube_playlist_generator_pro.py
   ```

3. **Run the `.exe`**:
   - Find the executable in `dist/youtube_playlist_generator_pro.exe`.
   - Double-click to run, or use:
     ```bash
     dist\youtube_playlist_generator_pro.exe
     ```

4. **Verify**:
   - Config and logs are in `C:\Users\<User>\AppData\Roaming\YouTubePlaylistGenerator`.
   - The icon appears in File Explorer, taskbar, and app window.

## Troubleshooting 🐛
- **PyInstaller Not Found**:
  ```bash
  python -m PyInstaller --onefile --windowed --icon=app_icon.ico youtube_playlist_generator_pro.py
  ```
- **Missing Dependencies**:
  Reinstall required packages:
  ```bash
  pip install requests google-api-python-client tenacity pyperclip Pillow isodate appdirs
  ```
- **Icon Not Applied**:
  Ensure `app_icon.ico` is valid and in the script’s directory.
- **Large `.exe` Size**:
  Use UPX to compress:
  ```bash
  pyinstaller --onefile --windowed --icon=app_icon.ico --upx-dir path_to_upx youtube_playlist_generator_pro.py
  ```

## Contributing 🤝
Got ideas? Open an issue or submit a pull request! Feature requests, bug fixes, or UI tweaks are welcome.

## License 📜
MIT License. See [LICENSE](LICENSE) for details.

## Acknowledgments 🙌
- Built with [Tkinter](https://docs.python.org/3/library/tkinter.html) for the GUI.
- Powered by [YouTube Data API](https://developers.google.com/youtube/v3) and [appdirs](https://pypi.org/project/appdirs/) for portability.
- Inspired by the need for quick, reliable playlist generation.

---

**Rock your YouTube playlists like a pro!** If you love this tool, give it a ⭐ on GitHub! 😈
