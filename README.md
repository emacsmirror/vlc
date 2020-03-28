# VideoLAN VLC Media Player Control
[![Melpa](https://melpa.org/packages/vlc-badge.svg)](https://melpa.org/#/vlc)

This package lets you control VLC through the [Web Interface](https://wiki.videolan.org/Control_VLC_via_a_browser/)'s [API](https://github.com/videolan/vlc/blob/fad0d14618f7be34b04347e517644764d43d8dad/share/lua/http/requests/README.txt).

## Usage

### Start VLC with the web interface

Go to Preferences → HTTP web interface → check "Enable HTTP web interface", and
don't forget to set a non-empty password, then restart VLC.

Another choice is simply `M-x vlc-start`, it will launch VLC for you with this
command:

    vlc --extraintf http --http-password secret

### Have fun

There are many commands such as `M-x vlc-add` to add a file to the playlist and
play it, here's a list of all commands:

- vlc-add
- vlc-clear
- vlc-delete
- vlc-empty
- vlc-enqueue
- vlc-fullscreen
- vlc-key
- vlc-loop
- vlc-next
- vlc-pause
- vlc-play
- vlc-prev
- vlc-random
- vlc-repeat
- vlc-seek
- vlc-snapshot
- vlc-sort
- vlc-stop
- vlc-volume

## Requires

- Emacs 25.1
- VLC

## Resources

- HTTP Requests API [README](https://github.com/videolan/vlc/blob/fad0d14618f7be34b04347e517644764d43d8dad/share/lua/http/requests/README.txt)
- API source code [httprequests.lua](https://github.com/videolan/vlc/blob/fad0d14618f7be34b04347e517644764d43d8dad/share/lua/intf/modules/httprequests.lua)
- Racket package https://docs.racket-lang.org/vlc/ for inspiration, it uses RC interface, not the Web Interface
