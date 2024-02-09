# <img src="https://i.ibb.co/z5yQMjZ/1000021078-removebg.png" width="28px" /> YTKD-MusicDownloaderPlayer
<div align="center">
  <img width="450" src="https://i.ibb.co/z5yQMjZ/1000021078-removebg.png">
</div>



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
  - Presents an interactive menu to the user with options to download a song, listen to a song, view popular songs, get lyrics, or exit the program.
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

- [x] **View Popular Songs:**
  - Users can explore a list of popular songs.
  - Fetches data from [Last.fm API](https://www.last.fm/api) to display top tracks.

- [x] **Get Lyrics of a Song:**
  - Users can retrieve the lyrics of a specific song.
  - Utilizes the [Genius API](https://docs.genius.com/) to fetch song lyrics.


> [!TIP]
> ███████████ API Keys Configuration ███████████
> 
>
> This project uses various APIs to obtain specific functionalities. Before proceeding, make sure to obtain the necessary API keys from their respective sites and replace the following placeholders with your keys.
> - **Last.fm API Key**: To get an API key from Last.fm, follow these steps:
> 1. Visit the Last.fm website ([https://www.last.fm/api/account/create](https://www.last.fm/api/account/create)) and sign in or create an account.
> 2. After logging in, go to the API console page ([https://www.last.fm/api/account/create](https://www.last.fm/api/account/create)).
> 3. Create a new project to obtain your API key.
> 4. Insert your API key in place of `Lastfmapi` in the following code:
>
>   ```python
>  LASTFM_API_KEY = 'Lastfmapi'
  > ```
>
> - **Genius API Key**: To get an API key from Genius, follow these steps:
>  1. Visit the Genius website ([https://genius.com/api-clients](https://genius.com/api-clients)) and sign in or create an account.
>  2. After logging in, create a new application to obtain your API key.
 > 3. Insert your API key in place of `genius-api` in the following code:
>
 >   ```python
  >  GENIUS_API_KEY = "genius-api"
   > ```
>
> Make sure to keep your API keys confidential and not share them publicly. For better security management, consider using environment variables or other secure methods to handle keys in your project.




> ## <img src="https://s13.gifyu.com/images/SC4KY.gif" width="45px" /> Dependencies

> [!IMPORTANT]
> # <img src="https://i.ibb.co/G9FRzt5/musical-note.png" width="45px" /> Installation of _**mpg123**_ and _**ImageMagick**_
>
> ## Prerequisites
> 🔐 _Make sure you have administrator privileges (sudo) to execute the installation operations._
>
> ## Installation
>
> | Distribution   | Installation Commands                                          |
> | -------------- | ------------------------------------------------------------- |
> | Ubuntu/Debian  | `sudo apt-get update`<br>`sudo apt-get install mpg123`<br>`sudo apt-get install imagemagick` |
> | CentOS/RHEL    | `sudo yum install epel-release`<br>`sudo yum install mpg123`<br>`sudo yum install ImageMagick` |
> | Fedora         | `sudo dnf install mpg123`<br>`sudo dnf install ImageMagick` |
> | Arch Linux      | `sudo pacman -S mpg123`<br>`sudo pacman -S imagemagick` |
> | openSUSE       | `sudo zypper install mpg123`<br>`sudo zypper install ImageMagick` |
> | Alpine Linux    | `sudo apk add mpg123`<br>`sudo apk add imagemagick` |
>
> ## Installation Verification
> ```bash
> mpg123 --version
> convert --version
> ```
>
> Ensure the above commands return information about the installed software to confirm a successful installation.

> [!WARNING]
> # 🎵 `ffmpeg` Requirement for `yt_dlp` 🚀
> 
> If you encounter the error `yt_dlp.utils.DownloadError: ERROR: Postprocessing: ffprobe and ffmpeg not found. Please install or provide the path using --ffmpeg-location`, ensure that 🎵 ffmpeg is installed on your system.
> 
> ## Installing 🎵 ffmpeg 🛠️
> 
> To install 🎵 ffmpeg, use the following commands based on your distribution:
> 
> | Distribution   | Installation Commands                        |
> | -------------- | ------------------------------------------- |
> | Ubuntu/Debian  | `sudo apt-get update`🔄<br>`sudo apt-get install ffmpeg`🎵 |
> | CentOS/RHEL    | `sudo yum install epel-release`🔄<br>`sudo yum install ffmpeg`🎵 |
> | Fedora         | `sudo dnf install ffmpeg`🎵 |
> | Arch Linux      | `sudo pacman -S ffmpeg`🎵 |
> | openSUSE       | `sudo zypper install ffmpeg`🎵 |
> | Alpine Linux    | `sudo apk add ffmpeg`🎵 |
> 
> ## Verification of Installation 🔍
> ```bash
> 🎵 ffmpeg --version
> ```
> 
> Ensure the above command returns information about the installed 🎵 ffmpeg version to prevent the mentioned error message.
> 
> 🚨 **Note:** _*This step is necessary to ensure the proper functioning of yt_dlp. Verify that 🎵 ffmpeg is installed or provide the path using the --ffmpeg-location option.*_ 🌟





> [!NOTE]
> _**Commands may vary based on specific distribution versions. Be sure to refer to your distribution's official documentation for any differences.**_



| Dependency                               | Description                                                                                                   |
|------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| [yt_dlp](https://github.com/yt-dlp/yt-dlp)       | A powerful and flexible library for downloading videos and audio from YouTube. 🎥🎵                                 |
| [rich](https://github.com/willmcgugan/rich)       | A library to enhance text formatting in the terminal, offering advanced colors and styles. 🌈✨                    |
| [pydub](https://github.com/jiaaro/pydub)          | A library for audio file manipulation. In Console Music Player, it is used to load and get information about song durations. 🎶  |
| [kitty](https://github.com/kovidgoyal/kitty)      | An advanced terminal emulator that supports direct image display. Used by Console Music Player to show animated GIFs. 🐱🖼️        |
| [mpg123](https://www.mpg123.de/)                 | A fast, free, and high-quality command-line MP3 player. Used by Console Music Player for song playback. 🎶🔊                      |
| [ImageMagick](https://imagemagick.org/)          | A powerful software suite for image editing and conversion. Used by Console Music Player, alongside mpg123, to enhance functionality. 🖼️✂️  |
| [ffmpeg](https://ffmpeg.org/)                    | A cross-platform solution for handling multimedia data. Utilized by Console Music Player for various audio and video processing tasks. 🎬🔧 |
| [lyricsgenius](https://pypi.org/project/lyricsgenius/)           | API for fetching song lyrics. Utilized by Console Music Player to retrieve lyrics of a specific song. 📜🎤 |
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








