

```latex
\documentclass[a4paper,11pt]{article}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{geometry}
\geometry{margin=1in}
\usepackage{hyperref}
\hypersetup{colorlinks=true, linkcolor=blue, urlcolor=blue}
\usepackage{enumitem}
\usepackage{titling}
\usepackage{fancyhdr}
\pagestyle{fancy}
\fancyhf{}
\fancyfoot[C]{\small Built with passion for YouTube enthusiasts. Turn videos into playlists like a pro!}
\renewcommand{\headrulewidth}{0pt}

\title{YouTube Playlist Generator Pro}
\author{}
\date{}

\begin{document}

\maketitle

\begin{center}
    \textbf{A powerful Windows app to transform YouTube video URLs into channel playlist URLs with ease!}
\end{center}

\section*{Introduction}
Welcome to \textbf{YouTube Playlist Generator Pro}, a standalone Windows application that converts any YouTube video URL into a full channel playlist URL in seconds. Whether you're curating playlists for binge-watching, studying, or sharing, this tool offers a sleek interface, video previews, duration estimates, and secure settings management. Perfect for YouTube enthusiasts!

\section*{Features}
\begin{itemize}[leftmargin=*]
    \item \textbf{Instant Playlist Generation}: Convert a YouTube video URL into a channel playlist URL effortlessly.
    \item \textbf{Video Previews}: View thumbnails, titles, channels, and durations for each input video.
    \item \textbf{Batch Processing}: Process multiple URLs at once for maximum efficiency.
    \item \textbf{Duration Estimates}: Get estimated playlist durations (requires a YouTube API key).
    \item \textbf{Customizable Filters}: Set minimum/maximum video counts and toggle strict filtering.
    \item \textbf{Dark Mode}: Switch between light and dark themes for a comfortable experience.
    \item \textbf{Secure Settings}: Store your YouTube API key safely in a password-masked settings dialog.
    \item \textbf{Export \& Copy}: Save playlist URLs to CSV or copy them to your clipboard.
    \item \textbf{Robust Error Handling}: Logs errors to a file for easy troubleshooting.
    \item \textbf{Portable}: Config and logs are stored in \texttt{C:\textbackslash Users\textbackslash<User>\textbackslash AppData\textbackslash Roaming\textbackslash YouTubePlaylistGenerator}.
\end{itemize}

\section*{Installation}
\begin{enumerate}[leftmargin=*]
    \item \textbf{Download the \texttt{.exe}}: Grab \texttt{youtube\_playlist\_generator\_pro.exe} from the \href{https://github.com/<your-username>/<your-repo>/releases}{Releases} page.
    \item \textbf{Run the App}: Double-click \texttt{youtube\_playlist\_generator\_pro.exe} to launch. No installation required!
    \item \textbf{Optional: Unblock the \texttt{.exe}}: Windows may flag the \texttt{.exe} as unknown. Right-click, select ``Properties,'' and click ``Unblock'' if the option appears.
\end{enumerate}

\section*{Usage}
\begin{enumerate}[leftmargin=*]
    \item \textbf{Launch the App}: Run \texttt{youtube\_playlist\_generator\_pro.exe}. The app opens in a compact, resizable window ($\sim$700x500 pixels).
    \item \textbf{Enter YouTube URLs}: Paste one or more YouTube video URLs (one per line, e.g., \texttt{https://www.youtube.com/watch?v=7r0CHuqRkI8}) in the ``YouTube Video URL(s)'' text area. Previews appear in the ``Video Previews'' pane.
    \item \textbf{Configure Settings}: Click \textbf{Settings > Configure Settings} in the menu bar. Enter a YouTube API key (optional) and toggle:
        \begin{itemize}
            \item \textbf{Include YouTube Shorts}: Include or exclude Shorts in playlists.
            \item \textbf{Dark Mode}: Enable for a sleek dark theme.
            \item \textbf{Request Timeout}: Set network timeout (5--30 seconds).
            \item \textbf{Min/Max Playlist Videos}: Filter playlists by video count (1--1000 min, 1--10000 max).
            \item \textbf{Enforce Video Count Filters}: Skip playlists that don’t meet count criteria.
        \end{itemize}
        Click ``Save'' to store settings in \texttt{C:\textbackslash Users\textbackslash<User>\textbackslash AppData\textbackslash Roaming\textbackslash YouTubePlaylistGenerator\textbackslash yt\_playlist\_config.json}.
    \item \textbf{Generate Playlists}: Click \textbf{Generate Playlists} to process URLs. Playlists open in your default browser. View progress and logs in the ``Results'' pane.
    \item \textbf{Manage Output}: Copy URLs to clipboard, export to CSV, or clear input via the ``Clear Input'' button or \textbf{File > Clear Input}.
    \item \textbf{Scroll \& Resize}: Use the scrollbar or mouse wheel to navigate previews and logs. Resize the window (minimum 600x400 pixels).
\end{enumerate}

\section*{Requirements}
\begin{itemize}[leftmargin=*]
    \item \textbf{Operating System}: Windows 7, 8, 10, or 11.
    \item \textbf{Internet Connection}: Required for fetching video data and generating playlists.
    \item \textbf{YouTube API Key} (optional): For video previews and duration estimates. Get one at \href{https://console.developers.google.com/}{Google Cloud Console}.
\end{itemize}

\section*{Troubleshooting}
\begin{itemize}[leftmargin=*]
    \item \textbf{App Doesn’t Open}: Ensure you’re on Windows and have unblocked the \texttt{.exe}. Check \texttt{C:\textbackslash Users\textbackslash<User>\textbackslash AppData\textbackslash Roaming\textbackslash YouTubePlaylistGenerator\textbackslash yt\_playlist\_errors.log} for details.
    \item \textbf{No Previews or Durations}: Provide a valid YouTube API key in the settings dialog and verify your internet connection.
    \item \textbf{URLs Not Processing}: Ensure URLs are valid YouTube video links (e.g., \texttt{https://www.youtube.com/watch?v=...} or \texttt{https://youtu.be/...}). Check error logs in the app or log file.
\end{itemize}

\section*{FAQ}
\begin{itemize}[leftmargin=*]
    \item \textbf{Where are config and log files stored?} In \texttt{C:\textbackslash Users\textbackslash<User>\textbackslash AppData\textbackslash Roaming\textbackslash YouTubePlaylistGenerator} (\texttt{yt\_playlist\_config.json} for settings, \texttt{yt\_playlist\_errors.log} for errors).
    \item \textbf{Do I need a YouTube API key?} Optional. Without one, the app uses scraping, but previews and duration estimates require an API key.
    \item \textbf{Can I run this on macOS or Linux?} This \texttt{.exe} is Windows-only. Contact the developer for cross-platform versions.
    \item \textbf{Why does Windows flag the \texttt{.exe}?} Unsigned executables may trigger Windows Defender. Unblock the file or add an exception.
\end{itemize}

\section*{Contributing}
This is a standalone \texttt{.exe} release. For feature requests or bug reports, create an \href{https://github.com/<your-username>/<your-repo>/issues}{Issue} on GitHub.

\section*{License}
Distributed under the \href{https://github.com/<your-username>/<your-repo>/blob/main/LICENSE}{MIT License}. Use, share, and enjoy!

\section*{Contact}
Questions or ideas? Open an issue on \href{https://github.com/<your-username>/<your-repo>}{GitHub}. Let’s make playlist generation even better! \emoji{rocket}

\end{document}
```

