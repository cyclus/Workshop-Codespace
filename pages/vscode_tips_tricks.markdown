---
layout: default
title:  "VS Code Tips and Tricks in Codespaces" 
---

# Tips and Tricks 
for working with `VS Code` in GitHub Codespaces
This pages provides some tips and tricks for using `VS Code` while in a GitHub 
Codespace. 

## Caution
### Keyboard Shortcuts Overriden by Browser
  Regular users of `VS Code` may find that common keyboard shortcuts in 
  (e.g.,`Ctrl+n` to create a new file) are overidden in by the internet 
  browser keyboard shortcuts  (e.g., `Ctrl+n` to open a new window) when using 
  GitHub Codespaces. 
  So, be aware that the function of the keystroke for your web browser will 
  occur  when you execute it in the codespace. That is, if you press `Ctrl+n` while in the 
  GitHub Codespace, a new browser window will open and no new VS Code file will be created. 

## Improving efficiency
* To create an XML input file, like is used in Cyclus, you can use the XML 
  schema for Cyclus to autocomplete and autogenerate parts of the input file: 
  * Make sure to include the following at the top of your input file.

  {% highlight xml %}
  <?xml-model href="../schema/cyclus.rng"
             type="application/xml"
             schematypens="http://relaxng.org/ns/structure/1.0"?>
  {% end highlight}

  * Type in the top-level `<simulation> </simulation>` set of tags
  * When your cursor is between those top-level tags, you can type `<` and a 
  menu of options will appear of possible options for the next-level tags (e.g., 
  `<archetypes>`, `<facility>`, etc.). 
  * Typing `Ctrl+Space` can also show these 
  autofill options.
  * Then inside each of those tags, you can continue to use `<` to help identify 
    tags that can be included inside each level. 
* Use ``Ctrl+` `` to toggle between the terminal and the file editor space. 
* `code <file name>` is a terminal shortcut to open files in the `VS Code` file 
  editor. 
