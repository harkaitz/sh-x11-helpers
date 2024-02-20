X11 Helpers
===========

Implementation of something similar to PLAN9 plumber for X11/Windows.

## Windows.

Shortcuts can be slow, fasten:

    Taskkill /IM ApplicationFrameHost.exe /F

    or disable SuperFetch in Sysmain
    https://superuser.com/questions/426947/slow-windows-desktop-keyboard-shortcuts


## Help

txt-edit

    Usage: txt-edit < INPUT > OUTPUT
    
    Read from the standard input, edit and print to standard output.

txt-exec

    Usage: txt-exec < CODE
    
    Read command from the standard input and execute in another
    terminal.

txt-open

    Usage: txt-open < FILENAME
    
    Read filenames from standard input and open with x-open(1).

txt-save-link

    Usage: txt-save-link [NAME] < LINK
    
    Save link to "last" link file for x-link(1).

txt-search

    Usage: txt-search [TERM] [ENGINE]
    
    Show a list of searchers ("x-search--NAME TERM" commands) and
    search the term.

x-compat

    Usage: x-compat ...
    
    ... clip-get          : Print text in clipboard.
    ... clip-put          : Save to clipboard.
    ... exec CODE         : Execute code from standard input.
    ... dmenu [-p PROMPT] :
    ... error HEAD MSG    :
    ... progs REGEX       : List programs that match REGEX.

x-editor

    Usage: x-editor [-V][-a] [FILE]
    
    Open file with an [-a : advanced] text editor.
    
    Environment variables: XEDITOR, AEDITOR
    Known text editors: xedit, mousepad, notepad, emacs

x-link

    Usage: x-link -Ve | [CATEGORY [NAME]]
    
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
    Dependencies: dmenu, xterm

x-open

    Usage: x-open -V | -l | -m FILE | FILE
    
    Open a file or URL using the user's preferred application.
    
    To choose which program to use x-open executes the scripts
    in '/etc/x-open.d' and '~/.x-open.d' passing to them the file
    or URL. Each line they return is a posible command.
    
    You can list the scripts with -l and the menu with -m FILE.

x-pipe

    Usafe: x-clip [COMMAND]
    
    Pipe the content in the clipboard to command and put it's output
    in the clipboard. If no command is specified it is asked with
    dmenu.

x-search

    Usage: x-search TERM

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
