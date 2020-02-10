---
layout: post
title: "Keyboard Centered Workflow on Windows 8"
---

Over the summer at my internship, I ran into some trouble with my laptop's wireless under Arch Linux.
Every five to ten minutes, the connection would cut out entirely and the SSID would disappear from the list,
reappearing after ten minutes of refreshing. None of my coworkers were having any trouble with their linux
wireless, and I could connect fine to any other network. After a few days of troubleshooting (reading forum
threads is slightly complicated by a lack of stable connection), I decided I'd have to go back to Windows.

Out of the box, Windows is pretty terrible for development, especially coming from a tiling window manager
on Linux. With some third-party software, though, Windows can be pretty ...alright.

## Virtual Desktops

The single biggest feature I miss in Windows, and one that any sane environment has, is virtual desktops.
The idea is straightforward: instead of having a single desktop holding all of your running applications,
you have multiple "workspaces" between which you split them, useful if you intend on ever doing more than
one thing at a time.

To this end, I have [Dexpot](http://dexpot.de/) set up with the following basic keybindings: `Alt-[number]`
to switch to that desktop, and `Alt-Shift-[number]` to move the active window to that desktop. I also enabled
the `Taskbar Pager` plugin for a nice visual indicator.

With virtual desktops, I find I have far fewer windows per desktop, so I don't need the window grouping
introduced in 7. `Taskbar > Properties > Taskbar buttons: Combine when taskbar full`, and `Use small taskbar
buttons` for the extra bit of vertical screen space.

## Window Tiling

Another killer feature I need in a window manager is the ability to place windows without touching the mouse.
Windows 7+ includes the shortcuts `Super-[arrow]` to place windows half left, half right, or maximized, but
that's rather limited.

[Winsplit Revolution](http://winsplit-revolution.com/) is a simple program that provides
shortcuts for placing windows into a variety of tile positions. By default, shortcuts are mapped to
`Ctrl-Alt-[numpad]`, forming a nine number grid, but since my laptop has no numpad I've remapped these to
`Ctrl-Alt-[left/right]` for either side, `Super-Alt-[left/right]` for the top half of either side,
`Super-Ctrl-[left/right]` for the lower half of either side, and `Ctrl-Alt-Down` to center. For working with 
multiple monitors, `Ctrl-Alt-n` moves a window to the right monitor, and `Ctrl-Alt-b` moves it to the left.

This makes for quick on-demand tiling, as shown:
![Tiling example](/public/tilingexample.png) 

Entering a shortcut once will place the window in the respective location, a second will shrink to one third
the horizontal screen space, and a third will grow to two thirds the space.

## Program Launching

Juggling windows via keyboard would be a lot less effective if I still had to fall back to mouse to launch
them, of course. My main two programs, Chrome and Cygwin, I have pinned to the taskbar, making them accessible with `Super-[1/2]`.

For everything else, the application launcher [Launchy](http://www.launchy.net/) (also available through
[Ninite](http://ninite.com/)), bound to `Alt-Space`, can handle files and programs.