<div align="center">
<h1>This is a little showcase</h1>
Click on the image for video. <a href="https://github.com/ccanvas/libccanvas/tree/master/examples/explorer">How this is made.</a>

[![](https://gmtex.siri.sh/api/usercontent/v1/file/id/1/tex/Dump/Showcases/ccanvas-explorer.png)](https://gmtex.siri.sh/fs/1/Dump/Showcases/ccanvas-explorer.webm)

<i>A fresh approach to TUI development that promotes efficiency and code reusability.</i>
</div>

## Why?

- Unlike traditional TUI programs that rely on a single binary with duplicated interface implementations, ccanvas allows **multiple binaries to draw on the same terminal**.
- In ccanvas, **binaries become reusable building blocks**, the same binary "component" can be employed across different "component bundles," eliminating duplicated implementations and promoting a modular approach to TUI development.

## How?

- Binary components **connect to ccanvas via Unix sockets**, enabling them to draw on the terminal and listen to events.
- Components can communicate with each other through messages, shared variables, and shared file storage.

## What?

Ok, so what does ccanvas in action looks like?

### Core

At its core, ccanvas is a program that provides a standardised interface for easy interaction.

- [**`ccanvas`**](https://github.com/ccanvas/ccanvas) - the main ccanvas program.
- [**`libccanvas`**](https://github.com/ccanvas/libccanvas) - binding structs + component utility.

> To create a component for ccanvas, visit [**`libccanvas/examples`**](https://github.com/ccanvas/libccanvas/tree/master/examples).

### Components

Components are the building blocks of a ccanvas program. Here are some general purpose components.

- [**`ccanvas-layout`**](https://github.com/ccanvas/ccanvas-layout) - component layout manager.
- [**`ccanvas-quit`**](https://github.com/ccanvas/ccanvas-quit) - configurable quitting handler.
- [**`ccanvas-saver`**](https://github.com/ccanvas/ccanvas-saver) - terminal size limiter/screen saver.
- [**`ccanvas-scroll`**](https://github.com/ccanvas/ccanvas-scroll) - scrolling text display.
- [**`ccanvas-solid`**](https://github.com/ccanvas/ccanvas-solid) - debug component to fill screen with the same character.

### Apps (component bundles)

A ccanvas reimplementation of [**`youtube-tui`**](https://github.com/Siriusmart/youtube-tui/) is currently being developed.

![image](https://github.com/ccanvas/.github/assets/71584876/9d48f08a-8e1d-493f-9fff-06c1494abf19)

Meanwhile, you can check out the minimal apps in [**`libccanvas/examples`**](https://github.com/ccanvas/libccanvas/tree/master/examples) to get a feel of its full power.

---

<div align="center">
  <code><3</code>
</div>

