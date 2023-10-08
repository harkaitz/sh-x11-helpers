# X11 HELPERS

Small utilities for the X11 desktop. It requires dmenu(1) and X11
utilities. I use this scripts for personal productivity.

## Help

dmenu-fsel

    Usage: dmenu-fsel [-n NAME][-C DIRECTORY][-c COMMAND,...]
    
    Select a file or a command using dmenu. The return value can
    be: "file FILENAME" or "COMMAND DIRECTORY"
    
    Dependencies: dmenu

x-auto

    Usage: x-auto -V
    
    Define scripts in "/etc/x-auto" with X11 automatizations with
    xdotool(1) and launch them with "x-auto".
    
    Dependencies: dmenu, xdotool

x-clip-clean

    Usage: x-clip-clean
    
    Clean selection from trash.
    
    Dependencies: xclip

x-clip-edit

    Usage: x-clip-edit
    
    Edit clipboard content.
    
    Dependencies: xclip

x-clip-exec

    Usage: x-clip-exec
    
    Execute the commands in the clipboard.
    
    Dependencies: xclip, xterm

x-clip-open

    Usage: x-clip-open
    
    Open the file in clipboard.
    
    Dependencies: x-open, xclip

x-clip-pipe

    Usafe: x-clip-pipe [COMMAND]
    
    Pipe the content in the clipboard to command and put it's output
    in the clipboard. If no command is specified it is asked with
    dmenu.
    
    Dependencies: xclip, dmenu

x-clip-trans

    Usage: x-clip-trans
    
    Translate the text inside the clipboard.
    
    Dependencies: xclip, xmessage

x-color

    Usage: x-color
    
    Select a point in the screen and copy it's color value
    with the #RRGGBB format.
    
    Dependencies: xclip, grabc

xdg-pipe

    Usage: xdg-pipe [-s SUFFIX][-p PROGRAM] < FILE
    
    Read from the standard input to a temporary file, and
    then open with `xdg-open(1)` or another program.
    
    Dependencies: xdg-pipe, xdg-open

x-editor

    Usage: x-editor [-V][-a] [FILE]
    
    Open file with an [-a : advanced] text editor.
    
    Environment variables: MEDITOR, XEDITOR
    
    Known text editors: xedit, mousepad, notepad, emacs

x-keyboard

    Usage: x-keyboard OPS...
    
    Configure keyboard shortcuts for XFCE.
    
      -V  : Show configuration.
      -l  : List keyboard shortcuts.
      -iX : Install XFCE keyboard shortcuts.
    
    Environment variables: X_KEYBOARD

x-link

    Usage: x-link -V | [CATEGORY [NAME]]
    
    Save your links in text format and access them using dmenu.
    
    File format   : NAME [ ; DESCRIPTION ] ; COMMAND
    File location : ${X_LINK_DIRECTORY}/CATEGORY
    
    Dependencies: xdg-open, dmenu

x-menu

    Usage: x-menu [-Vl]
    
    Show a menu with dmenu of a selection of commands in "~/.x-menu".
    
    The list follows the following convention: "CMD : DESC [{w,f,t}]".
    - w : Commands that window themselves.
    - f : Command line programs, keep xterm open 2 seconds after finishing.
    - t : Wait an enter after finishing.
    
    Environment variables: X_MENU

x-monitor

    Usage: x-monitor PROGRAM ARGS...
    
    Execute program in the background in another xterm session. If
    the file changes restart the program.
    
    Dependencies: xterm, notify-send(optional)

x-note

    Usage: x-note -V | ...
    
    ... n NAME      : Create new notes file.
    ... NAME d      : Delete notes file.
    ... NAME a TAKE : Add new take.
    ... NAME p      : Print take (and copy to clipboard)
    
    Dependencies: dmenu, x-editor

x-open

    Usage: x-open -V | -l | -m FILE | FILE
    
    Open a file or URL using the user's preferred application.
    
    To choose which program to use x-open executes the scripts
    in '/etc/x-open' and '~/.local/etc/x-open' passing to them
    the file or URL. Each line they return is a posible command.
    
    You can list the scripts with -l and the menu with -m FILE.

x-postit

    Usage: x-postit [-V][NOTE]
    
    Dependencies: dmenu, x-editor

x-report

    Usage: x_report [-nl] [NOTE]
    
    Directories: "$X_REPORT_DIR", "~/Documents/X_Report"

x-screenshot

    Usage: x-screenshot
    
    Select a window and take a screenshot.
    
    Dependencies: xdotool, xdg-open

x-search

    Usage: x-search [TERM]

x-todo

    Usage: x-todo ...
    
    Daily TODO task management utility.
    
      -V : Show configuration.
      -E : Edit todo template list.
      -e : Open todo file.
      -a : Add todo lines from template.

x-wiki

    Usage: x-wiki [-V] : Open/create notes.
    
    Environment variables: X_WIKI_DIRECTORY
    Dependencies: dmenu, xmessage, x-editor

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
