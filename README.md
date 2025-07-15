YouTube Playlist Generator Pro
Welcome to YouTube Playlist Generator Pro, a powerful Windows app that transforms any YouTube video URL into a full channel playlist URL with ease! 🚀 Whether you’re curating playlists for binge-watching, studying, or sharing, this standalone .exe makes it simple, fast, and secure. With video previews, duration estimates, and a sleek interface, it’s your go-to tool for YouTube playlist magic.
Features 🎥

Instant Playlist Generation: Enter a YouTube video URL, and get a playlist URL for the entire channel in seconds.
Video Previews: See thumbnails, titles, channels, and durations for each input video.
Batch Processing: Process multiple URLs at once for ultimate efficiency.
Duration Estimates: Get estimated playlist durations (requires a YouTube API key).
Customizable Filters: Set minimum/maximum video counts and toggle strict filtering.
Dark Mode: Switch between light and dark themes for a comfy viewing experience.
Secure Settings: Store your YouTube API key safely in a password-masked settings dialog.
Export & Copy: Save playlist URLs to CSV or copy them to your clipboard.
Robust Error Handling: Logs errors to a file for easy troubleshooting.
Portable: Config and logs are stored in C:\Users\<User>\AppData\Roaming\YouTubePlaylistGenerator, so the .exe works anywhere.

Installation 📦

Download the .exe:

Grab youtube_playlist_generator_pro.exe from the Releases page.


Run the App:

Double-click youtube_playlist_generator_pro.exe to launch.
No installation required—just run it from any folder!


Optional: Unblock the .exe:

Windows may flag the .exe as unknown. Right-click, select “Properties,” and click “Unblock” if the option appears.



Usage 🎬

Launch the App:

Run youtube_playlist_generator_pro.exe. The app opens with a compact, resizable window.


Enter YouTube URLs:

In the “YouTube Video URL(s)” text area, paste one or more YouTube video URLs (one per line, e.g., https://www.youtube.com/watch?v=7r0CHuqRkI8).
Previews (thumbnails, titles, channels, durations) appear instantly below.


Configure Settings:

Click Settings > Configure Settings in the menu bar.
Enter a YouTube API key (optional, for duration estimates and enhanced previews).
Toggle options:
Include YouTube Shorts: Include or exclude Shorts in playlists.
Dark Mode: Enable for a sleek dark theme.
Request Timeout: Set network timeout (5–30 seconds).
Min/Max Playlist Videos: Filter playlists by video count.
Enforce Video Count Filters: Skip playlists that don’t meet count criteria.


Click “Save” to store settings in C:\Users\<User>\AppData\Roaming\YouTubePlaylistGenerator\yt_playlist_config.json.


Generate Playlists:

Click Generate Playlists to process URLs.
Playlists open in your default browser.
View progress and logs in the “Results” pane.


Manage Output:

Copy URLs: Click to copy generated playlist URLs to your clipboard.
Export URLs: Save original and playlist URLs to a CSV file.
Clear Input: Reset the URL input and previews.


Scroll & Resize:

Use the scrollbar or mouse wheel to navigate previews and logs.
Resize the window (minimum 600x400 pixels) for your preferred layout.



Requirements 🖥️

Operating System: Windows 7, 8, 10, or 11.
Internet Connection: Required for fetching video data and generating playlists.
YouTube API Key (optional): For video previews and playlist duration estimates. Get one at Google Cloud Console.

Troubleshooting ⚙️

App Doesn’t Open:

Ensure you’re on Windows and have unblocked the .exe (see Installation).
Check C:\Users\<User>\AppData\Roaming\YouTubePlaylistGenerator\yt_playlist_errors.log for error details.


No Previews or Durations:

Provide a valid YouTube API key in the settings dialog.
Check your internet connection.


URLs Not Processing:

Ensure URLs are valid YouTube video links (e.g., https://www.youtube.com/watch?v=... or https://youtu.be/...).
View error logs in the app or log file.



FAQ ❓
Q: Where are config and log files stored?A: In C:\Users\<User>\AppData\Roaming\YouTubePlaylistGenerator (yt_playlist_config.json for settings, yt_playlist_errors.log for errors).
Q: Do I need a YouTube API key?A: Optional. Without one, the app falls back to scraping, but previews and duration estimates require an API key.
Q: Can I run this on macOS or Linux?A: This .exe is Windows-only. Contact the developer for cross-platform versions.
Q: Why does Windows flag the .exe?A: Unsigned executables may trigger Windows Defender. Unblock the file or add an exception.
Contributing 🤝
This is a standalone .exe release. For feature requests, bug reports, or feedback, create an Issue on GitHub.
License 📜
This project is distributed as a standalone executable under the MIT License. Use it, share it, and enjoy!
Contact 📬
Got questions or ideas? Open an issue or reach out via GitHub. Let’s make playlist generation even better! 🎉

Built with 💪 for YouTube enthusiasts. Turn videos into playlists like a pro!
