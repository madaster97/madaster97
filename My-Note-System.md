# Note Taking:
Love this guy's note-taking approach:

## Mischa van den Burg
https://mischavandenburg.com/zet/neovim-zettelkasten/
https://www.youtube.com/watch?v=Xw3SkhB4dMk

> I have a directory structure based on the [PARA method](https://fortelabs.com/blog/para/), but I also have a large Zettelkasten directory where I put anything that does not necessary belong to a category.

> I recommend [this article](https://rwx.gg/lang/md/) about the benefits and merits of using markdown for note-taking.

### Principles
- Structure and intention!
- Understand through writing

## Helpful Links
[VSCode VIM Extension](https://github.com/VSCodeVim/Vim/blob/HEAD/ROADMAP.md)
[Relative Line #s](https://stackoverflow.com/questions/4967217/relative-line-numbers-in-visual-studio)
[MARKSMAN LSP](https://github.com/artempyanykh/marksman-vscode)

## Helpful VSCode Hotkeys
`CTRL + SHIFT + P` - Open command palette (then search for "Markdown Preview")
`CTRL + SHIFT + E` - Hop to file explorer/back\
`SHIFT + ALT + F` - Search in selected folder\
`CTRL + B` - Close the file explorer sidebar

https://code.visualstudio.com/docs/editor/editingevolved

## More Hotkeys
Close Sidebar - `CTRL + B`

## What I've Done
- Installed Marksman VSCode extension
- Installed Pandoc (no VSCode extension just CLI it)
- Have VSCode previewing MD 


### Marksman
Remember .marksman.toml!\
Check out their [features](https://github.com/artempyanykh/marksman/blob/main/docs/features.md#workspace-folders-project-roots-and-single-file-mode)\
[Config available](https://github.com/artempyanykh/marksman/blob/main/Tests/default.marksman.toml) includes *title_from_heading*
Remember *Ambiguous link to document* - Default config is not allow multiple top-level headings
_TODO_ - Figure out reference links + how to view/navigate + wiki linking

## Resources
### Titus Tech
https://www.youtube.com/watch?v=ZR_Kjg9GIBM


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

### Markdown Note Taking
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

### Neovim
*Didn't do this, just VSCode*

Combine Mischa's stuff with this neovim on windows article (like glyphs!)
https://blog.nikfp.com/how-to-install-and-set-up-neovim-on-windows

Consider Marksman LSP vs this Pandoc plugin?
https://github.com/vim-pandoc/vim-pandoc
