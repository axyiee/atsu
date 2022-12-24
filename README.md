# atsu

Watch YouTube and anime from the command line

## Installation

**Requirements:**

-   bash
-   [pup] - HTML parsing and extraction tool
-   [jq] - JSON parsing tool
-   [aria2] - Download manager
-   [mpv] or any other video player

[pup]: https://github.com/ericchiang/pup
[jq]: https://stedolan.github.io/jq/
[aria2]: https://aria2.github.io/
[mpv]: https://mpv.io/

```bash
git clone https://code.axyria.dev/atsu
doas cp ./atsu/atsu /usr/local/bin
```

## Usage

```bash
Usage: atsu [options]
Options:
  -h, --help            Show this help message and exit.
  -s, --search <term>   Search for anime episodes and play them.
  -i, --index <index>   The episode number to be searched on. You can set it to
                        'all' to search for all episodes.
  -p, --player <player> The media player used to play multimedia. Default is mpv,
                        or umpv if available.
# Example: atsu -s "one piece" -i 1
#          atsu -s "neon genesis evangelion" -i all -p vlc
```

## Extra

### YouTube Player

**Requirements:**

-   bash
-   [pup] - HTML parsing and extraction tool
-   [yt-dlp] - YouTube media downloader
-   [mpv] or any other video player
-   [xorg-xrandr] - X11 RandR extension client, used for extracting screen resolution

[yt-dlp]: https://github.com/yt-dlp/yt-dlp

You can also play YouTube videos by using an addon called `yatsu`! It works by scrapping content
from available Invidious instances. The usage is the same as `atsu`, without the `-i` option:

```bash
Usage: yatsu [options]
Options:
  -h, --help            Show this help message and exit.
  -s, --search <term>   Search for YouTube videos and play them.
  -p, --player <player> The media player used to play multimedia. Default is mpv,
                        or umpv if available.
```
