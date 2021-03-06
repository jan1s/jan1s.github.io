---
layout: post
title:  "LaTeX Toolchain"
date:   2016-11-26 18:44:26 +0100
categories: jekyll update
---

There are many ways to compile your LaTeX.
Here is how i do it.

# macOS

1. If you have not installed [Homebrew][brew] yet, you should do that right now.

2. Install [Cask][cask] for binary management:

    ```bash
    brew tap caskroom/cask
    ```

3. Install [MacTeX][mactex] LaTeX toolchain:

    ```bash
    brew cask install mactex
    ```

4. Install [Sublime Text][subl] text editor:

    ```bash
    brew cask install sublime-text
    ```

5. Install [skim][skim] PDF viewer:

    ```bash
    brew cask install skim
    ```

6. Install [ImageMagick][imagemagick] for equation preview (optional):

    ```bash
    brew install imagemagick
    brew install ghostscript
    ```

7. Install [Package Control][packagecontrol] in Sublime Text:
    
    Simply follow the on-site instructions


8. Install [LaTeXTools][latextools] plugin in Sublime Text:

    Press `⌘+⇧+P` in Sublime Text

    Enter `Package Control: Install Package`

    Enter `LaTeXTools`

Now you should be able to compile your .tex Documents with `⌘+B`


# Windows

1. Install [MiKTeX][miktex] LaTeX toolchain

2. Install [Sublime Text][subl] text editor

3. Install [Sumatra PDF][sumatra] reader

4. Install [Package Control][packagecontrol] in Sublime Text:
    
    Simply follow the on-site instructions


5. Install [LaTeXTools][latextools] plugin in Sublime Text:

    Press `Ctrl+Shift+P` in Sublime Text

    Enter `Package Control: Install Package`

    Enter `LaTeXTools`

Now you should be able to compile your .tex Documents with `Ctrl+B`




[brew]: http://brew.sh
[cask]: https://caskroom.github.io
[mactex]: http://www.tug.org/mactex/
[skim]: http://skim-app.sourceforge.net
[subl]: https://www.sublimetext.com
[imagemagick]: http://imagemagick.org
[packagecontrol]: https://packagecontrol.io/installation
[latextools]: https://github.com/SublimeText/LaTeXTools

[miktex]: https://miktex.org/download
[sumatra]: https://www.sumatrapdfreader.org