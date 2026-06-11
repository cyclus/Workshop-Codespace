# Tips and Tricks for working with VS Code in GitHub Codespaces
This pages provides some tips and tricks for using VS Code while in a GitHub 
Codespace. 

## Caution Items
* There are many keystroke shortcuts that you can use with VS Code when it is 
  installed on your computer (e.g., `Ctrl+n` to create a new file) that are 
  similar to keystrokes for using an internet browser (e.g., `Ctrl+n` to 
  open a new window). The function of the keystroke for your web browser will 
  occur  when in the codespace. E.g., if you press `Ctrl+n` while in the 
  codespace, a new browser window will open and no new file will be created. 

## Improving efficiency
* To create an XML input file, like is used in Cyclus, you can use the XML 
  schema for Cyclus to autocomplete and autogenerate parts of the input file: 
  * Make sure to have 
  ```
  <?xml-model href="../schema/cyclus.rng"
             type="application/xml"
             schematypens="http://relaxng.org/ns/structure/1.0"?>
  ```
  at the top of your input file.
  * Type in the top-level `<simulation> </simulation>` set of tags
  * When your cursor is between those top-level tags, you can type `<` and a 
  menu of options will appear of possible options for the next-level tags (e.g., 
  `<archetypes>`, `<facility>`, etc.). Typing `Ctrl+Space` can also show these 
  autofill options.
  * Then inside each of those tags, you can continue to use `<` to help identify 
    tags that can be included inside each level. 
* Use ``Ctrl+` `` to toggle between the terminal and the file editor space. 