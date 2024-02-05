# <img src="https://i.ibb.co/z5yQMjZ/1000021078-removebg.png" width="28px" /> YTKD-MusicDownloaderPlayer
<div align="center">
  <img width="450" src="https://i.ibb.co/z5yQMjZ/1000021078-removebg.png">
</div>

> [!IMPORTANT]
> [x] **This application is being finalized and will be released soon.**

> [!TIP]
> - The program utilizes the [yt_dlp](https://github.com/yt-dlp/yt-dlp), [rich](https://github.com/willmcgugan/rich), [pydub](https://github.com/jiaaro/pydub), and [kitty](https://github.com/kovidgoyal/kitty) libraries. Check their documentation for additional features and updates.


[![Python Version](https://img.shields.io/badge/python-3.9%20to%203.11-blue?logo=python)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
[![yt-dlp Downloading](https://img.shields.io/badge/yt--dlp-latest-brightgreen?logo=youtube)](https://github.com/yt-dlp/yt-dlp)
[![Rich Console Output](https://img.shields.io/badge/rich-latest-yellowgreen?logo=python)](https://github.com/willmcgugan/rich)
[![Audio Processing](https://img.shields.io/badge/pydub-latest-orange?logo=audio)](https://github.com/jiaaro/pydub)
[![MP3 Playback](https://img.shields.io/badge/mpg123-latest-brightred?logo=music)](https://www.mpg123.de/)

## <img src="https://s13.gifyu.com/images/SC4wb.gif" width="28px" /> Introduction
> # Music Downloader and Player

<img src="https://s13.gifyu.com/images/SC4w9.gif" width="400">

> Welcome to the **YTKD-MusicDownloaderPlayer** script! This Python script is designed for downloading and playing your favorite songs. It utilizes the [yt_dlp](https://github.com/yt-dlp/yt-dlp), [Rich](https://github.com/willmcgugan/rich), and [PyDub](https://github.com/jiaaro/pydub) libraries to enhance the user experience.


## <img src="https://s13.gifyu.com/images/SC4KY.gif" width="45px" /> Features


- [x] **Download a Song:**
  - Utilizes the `yt_dlp` library to download a song from YouTube.
  - Configurable options such as output format, audio quality, and download directory.

- [x] **View Downloaded Songs:**
  - Displays a list of downloaded songs in the "downloads" directory.
  - Utilizes the `rich` library to create a colorful table with song numbers and names.
  - Uses `pydub` to get the song duration and `kitty` to show a GIF during the listing.

- [x] **Play a Song:**
  - Uses `pydub` to load the MP3 file and get its duration.
  - Utilizes `subprocess` to start playing the song using `mpg123`.
  - Displays a colored panel with playback information such as song name and duration.
  - Shows remaining time during playback.
  - Playback stops when the song ends.

- [x] **Interactive Menu:**
  - Presents an interactive menu to the user with options to download a song, listen to a song, or exit the program.
  - Utilizes the `rich` library to display the menu with colors and styles.
  - Handles user choices through a while loop.

- [x] **Animated GIFs:**
  - Uses animated GIFs hosted on Gifyu to display animations during various operations (download, listing, menu).

- [x] **Colorful Interface:**
  - Uses the `rich` library to create colorful panels and formatted text in the terminal.
  - Utilizes a cyclic sequence of colors for various graphical elements.

- [x] **Styled Input Handling:**
  - Uses the `styled_input` function to obtain user input in a stylized way through the `rich` library.

- [x] **Modular Structure:**
  - Organized code into functions like `download_song`, `list_downloaded_songs`, `play_song`, `styled_input`, and `main` for a clearer and modular structure.

- [x] **Download Directory Creation:**
  - Checks if the "downloads" directory exists and creates it if it doesn't.

- [x] **Program Exit:**
  - Users can exit the program by selecting the corresponding option in the menu.

> ## <img src="https://s13.gifyu.com/images/SC4KY.gif" width="45px" /> Dependencies
| Dependency | Description                                                                                                   |
|------------|---------------------------------------------------------------------------------------------------------------|
| yt_dlp     | A powerful and flexible library for downloading videos and audio from YouTube.                                |
| rich       | A library to enhance text formatting in the terminal, offering advanced colors and styles.                     |
| pydub      | A library for audio file manipulation. In YTKD-MusicDownloaderPlayer, it is used to load and get information about song durations. |
| kitty      | An advanced terminal emulator that supports direct image display. Used by YTKD-MusicDownloaderPlayer to show animated GIFs.         |
| mpg123     | A fast, free, and high-quality command-line MP3 player. Used by YTKD-MusicDownloaderPlayer for song playback.                      |



> To ensure an optimal experience with **YTKD-MusicDownloaderPlayer**, make sure to have the following dependencies installed in your Python environment. You can do this easily by running the following command:

```bash
pip install -r requirements.txt
```

> [!TIP]
> - **Internet Connection:** Ensure a stable internet connection for smooth song downloads from YouTube.
> - **Audio Playback:** Make sure your system has audio playback capabilities, and the `mpg123` player is installed.
> - **GIF Display:** The program uses the `kitty` terminal emulator to display animated GIFs. Ensure your terminal supports image display.
> - **Directory Creation:** YTKD-MusicDownloaderPlayer will create a "downloads" directory if it doesn't exist. Make sure the program has write permissions.

> [!WARNING]
> - **Legal Considerations:** Respect copyright laws and YouTube's terms of service while using this tool. Ensure you have the right to download and play the content.
> - **Terminal Compatibility:** Some terminal emulators may not support certain features, such as GIF display. If you encounter issues, consider using a different terminal.
> - **GIF Loading Time:** The initial loading of GIFs may take some time, depending on your internet speed.

> [!IMPORTANT]
> - **Customization:** Feel free to customize the code to suit your preferences or add new features.
> - **Feedback:** If you encounter issues or have suggestions, please open an issue on GitHub.








