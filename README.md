Sublime Text 2 Build MarkDown
===============================

This is a fork of the [Markdown Preview][7] Sublime Text 2 plugin and a peice of the [Markdown Build][1] plugin to enable you to preview your Markdown files in the browser as well as save the HTML file that is generated in the same directory as the Markdown file, using the same filename with .html as the extension.

You can use builtin [python-markdown2][0] parser (default) or use the [github markdown API][5] for the conversion (edit your settings to select it). You can also choose between which CSS file to use: markdown.css, github.css or a CSS file of your choosing.

If you have the ST2 LiveReload plugin, your browser will autorefresh the display when you save your file :)

**NOTE:** If you choose the GitHub API for conversion (set parser: github in your settings), your code will be sent through https to github for live conversion. You'll have [Github flavored markdown][6], syntax highlighting and EMOJI support for free :heart: :octocat: :gift:

## Installation :

 - you should use [sublime package manager][3]
 - use `Ctrl + Shift + P` on Windows or `Cmd + Shift + P` on Mac then `Package Control: Install Package`
 - look for `BuildMarkdown` and install it.

## Usage :

 - use `Ctrl + Shift + B` or `Cmd + Shift + B` on Mac, then `BuildMarkdown` to launch a preview
 - or bind some key in your user key binding, using a line like this one:
   `{ "keys": ["alt+m"], "command": "build_markdown", "args": {"target": "browser"} },`
 - once converted a first time, the output HTML will be updated on each file save (with LiveReload plugin)

## Uses :

 - [python-markdown2][0] for markdown parsing **OR** the GitHub markdown API.


## Licence :

The code is available at github [https://github.com/jaredwilli/BuildMarkdown][2] under MIT licence : [http://mit-license.org][4]

 [0]: https://github.com/trentm/python-markdown2
 [1]: https://github.com/jfoshee/Markdown-Build
 [2]: https://github.com/jaredwilli/BuildMarkdown
 [7]: https://github.com/revolunet/sublimetext-markdown-preview
 [3]: http://wbond.net/sublime_packages/package_control
 [4]: http://revolunet.mit-license.org
 [5]: http://developer.github.com/v3/markdown
 [6]: http://github.github.com/github-flavored-markdown/
