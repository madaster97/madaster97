# Note Taking:

## What I've Done
- Have a *Notes* folder full of PARA-organized folders, take notes in [Markdown documents](#markdown-notetaking)
- Have VSCode for previewing and editing markdown, learned [hotkeys](#helpful-vscode-hotkeys-for-notetaking)
- Have [VSCode Vim Extension](#vim-motions-in-vs-code)
- Installed Marksman VSCode extension (see [below](#marksman)), to do things like:
  - `[[other-file-header]]` to reference other files and get hover text and CTRL+Click to open them. Quick plug for `gd` vim command (go to definition), **works in epiccode integration too** to open other routines! Use `gt` to go back to last file
  - `![Picture Description](picture-name.png]]` to reference pictures
    - When converting to MediaWiki, re-formats to create a link wiki recognizes, can click to quickly upload your image!
    - And if you keep your images next to your files, they get pulled into powerpoint just fine!
- Installed Pandoc (no VSCode extension just command line it)

## Mischa van den Burg Notetaking
Love this guy's note-taking approach:
- https://mischavandenburg.com/zet/neovim-zettelkasten/  
- https://www.youtube.com/watch?v=Xw3SkhB4dMk

> I have a directory structure based on the [PARA method](https://fortelabs.com/blog/para/), but I also have a large Zettelkasten directory where I put anything that does not necessary belong to a category.

> I recommend [this article](https://rwx.gg/lang/md/) about the benefits and merits of using markdown for note-taking.

### Principles
- Structure and intention
- Understand through writing

### PARA method
*Projects, Areas, Resources, Archive*

You have *projects* you’re actively working on – short-term efforts (in your work or personal life) that you take on with a certain goal in mind.

You have areas of *responsibility* – important parts of your work and life that require ongoing attention. These might include:

Then you have *resources* on a range of topics you’re interested in and learning about...

Finally, you have archives, which include anything from the previous three categories that is no longer active, but you might want to save for future reference:
- Projects you’ve completed or put on hold
- Areas that are no longer active or relevant
- Resources that you’re no longer interested in

It may be difficult to believe that a complex, modern human life like yours can be reduced to just four categories. It may feel like you have far more to deal with than can fit into such a simple system.
But that is exactly the point: if your organizational system is as complex as your life, then the demands of maintaining it will end up robbing you of the time and energy you need to live that life.

## Markdown Notetaking
[MARKSMAN LSP](https://github.com/artempyanykh/marksman-vscode)

Use Pandoc Markdown! Will have better mediawiki integration for sure (like nesting references to other docs)
- https://rwx.gg/lang/md/
- https://rwx.gg/lang/md/pandoc/
- https://pandoc.org/MANUAL.html#pandocs-markdown

### Pandoc Markdown to MediaWiki
Remember to `*` your lists, not `-`:
```powershell
pandoc --wrap=preserve -f markdown-smart "your markdown file here" -t mediawiki --ascii
```

References:
- [Wrap Preserve](https://stackoverflow.com/questions/63350182/pandoc-not-generating-new-lines-in-markdown-with-latex)
- [ascii for stupid quotes fix](https://github.com/jgm/pandoc/issues/7666)

### Pandoc Markdown to powerpoint
[Helpful Article](https://stymied.medium.com/what-slides-from-markdown-5239ed31e7ac)

If you have a bullet list and some text on one slide, need to **put a newline** after the text before the list

Planning a powershell script to open/close powerpoint from powershell, piping in my file:
<https://stackoverflow.com/questions/72747198/how-to-write-powershell-script-to-open-and-close-a-program>

```powershell
$exe = "C:\Program Files\Microsoft Office\root\Office16\POWERPNT.EXE"
```

## Vim Motions
Pretty convincing video on learning [Vim keyboard shortcuts/motions](https://youtu.be/sqm4-B07LsE?si=1Mc1AEm8Rrc1DFw5)

And here's [edgier guy](https://www.youtube.com/watch?v=X6AR2RMB5tE&list=PLm323Lc7iSW_wuxqmKx_xxNtJC_hJbQ7R) that wrote nice tutorials

### Vim Motions in VS Code
[VSCode VIM Extension](https://github.com/VSCodeVim/Vim/blob/HEAD/ROADMAP.md)
[Relative Line #s](https://stackoverflow.com/questions/4967217/relative-line-numbers-in-visual-studio)

### Helpful VSCode Hotkeys for Notetaking
`CTRL + SHIFT + P` - Open command palette (then search for "Markdown Preview")
`CTRL + SHIFT + E` - Hop to file explorer/back\
`SHIFT + ALT + F` - Search in selected folder\
`CTRL + B` - Close the explorer sidebar

https://code.visualstudio.com/docs/editor/editingevolved

Added a couple of my own:
- ([guide here](https://medium.com/vs-code-keybindings/keyboardizing-the-search-view-ac6026acea5b)): Made `enter` the hotkey to focus on search results (when in search results pane): `search.action.focusSearchList`. Otherwise you have to hit tab **13 times**
- Made `CTRL + SHIFT + U` put focus on search results pane. Helpful for hopping through lots of results. Vim j/k hotkeys let you navigate within the results

## Marksman
Remember .marksman.toml!  
Check out their [features](https://github.com/artempyanykh/marksman/blob/main/docs/features.md#workspace-folders-project-roots-and-single-file-mode)  
[Config available](https://github.com/artempyanykh/marksman/blob/main/Tests/default.marksman.toml) includes *title_from_heading*

Remember *Ambiguous link to document* - Default config is not allow multiple top-level headings

## Honorable Mentions

### Titus Tech
https://www.youtube.com/watch?v=ZR_Kjg9GIBM

### Neovim
*Didn't do this, just VSCode*

Combine Mischa's stuff with this neovim on windows article (like glyphs!)
https://blog.nikfp.com/how-to-install-and-set-up-neovim-on-windows

Consider Marksman LSP vs this Pandoc plugin?
https://github.com/vim-pandoc/vim-pandoc
