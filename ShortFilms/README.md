Stream from a selection of short films, powered by [Short of the Week](https://www.shortoftheweek.com/).

Run `shorts` and it’ll show a list of the latest films. Pick one and it’ll start streaming. Alternatively, use ⌘ to copy the short’s link to the clipboard or ⌥ to see its synopsis.

![](https://i.imgur.com/ntamau0.gif)

Short of the Week publishes a new short every day and building the initial list takes a few seconds, so after the initial download the list is cached for one day. If you want the list ready at all times without having to wait, run `:shortfilmslaunchd` to install (or later remove, running the same command) a `launchd` service to seamlessly update the list every day close to the time Short of the Week updates their website.

![](https://i.imgur.com/4fJTmJg.png)

Streaming is done with either `mpv` or `vlc`, depending on what you have (`mpv` takes precedence). For `mpv`, `youtube-dl` is a requirement; use the `youtube_dl_path` Workflow Environment Variable to set its path, if needed.
