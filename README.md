# atsu

Watch anime from the command line

## Installation

**Requirements:**

-   obviously, bash
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
  -s, --search <term>   Search for anime episodes and play it.
  -i, --index <index>   The episode number to be searched on. You can set it to
                        'all' to search for all episodes.
  -p, --player <player> The media player used to play the anime. Default is mpv,
                        or umpv if available.
# Example: atsu -s "one piece" -i 1
#          atsu -s "neon genesis evangelion" -i all -p vlc
```
