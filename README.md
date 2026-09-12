# MD Viewer

A local Markdown viewer. Run it from the command line, pick a folder, and browse your `.md` files in the browser.

![MD Viewer screenshot](https://github.com/user-attachments/assets/32ec484a-b3d2-40a6-b389-f4e4622b3a56)

## Usage

```bash
./mdview
./mdview /path/to/notes
```

That starts a local server, opens your browser, and remembers the last folder you opened. If nothing is saved yet, choose a folder in the UI.

Press `Ctrl+C` in the terminal to stop it.

`./mdview` is a small Python 3 script (stdlib only). A static HTML page cannot reliably read or remember a folder on disk, so Python serves the files locally and opens the browser. You do not need to install any packages.

## Features

- Shows `.md` and `.markdown` files in a collapsible directory tree
- Remembers collapsed directories between sessions
- Collapsible sidebar for comfortable reading in narrow and split-screen windows
- Automatically starts with the sidebar collapsed on narrow screens
- Renders GitHub-flavored Markdown with syntax highlighting
- Dark and light mode
- Remembers the last folder in `~/.mdview.json`
