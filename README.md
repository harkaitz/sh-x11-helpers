# X11 HELPERS

Small utilities for the X11 desktop. It requires dmenu(1) and X11
utilities.

## Help

x-auto

    Usage: x-auto -V
    
    Define scripts in "/etc/x-auto" with X11 automatizations with
    xdotool(1) and launch them with "x-auto".

x-clip-edit

    Usage: x-clip-edit
    
    Edit clipboard content.

x-clip-exec

    Usage: x-clip-exec
    
    Execute the commands in the clipboard.

x-clip-pipe

    Usafe: x-clip-pipe [COMMAND]
    
    Pipe the content in the clipboard to command and put it's output
    in the clipboard. If no command is specified it is asked with
    dmenu.

x-clip-trans

    Usage: x-clip-trans
    
    Translate the text inside the clipboard.

x-color

    Usage: x-color
    
    Select a point in the screen and copy it's color value
    with the #RRGGBB format.

x-phone

    Usage: x-phone [-V] COMMAND
    
    Execute a command inside a separate X11 server with a phone size.

x-record

    Start recording: x-record -av -o MKV-FILE
    Stop recording : x-record -s
    
    You can view configuration variables with "-V" and
    set them in "~/.x-record.cfg".

x-screenshot

    Usage: x-screenshot
    
    Select a window and take a screenshot.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
