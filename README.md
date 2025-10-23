# Ascend-Translations
This is the repository for translations of the Ascend game to different languages. All of the text and current translations are in `text.json`. That is the main and only configuration file for the text in the game. 

## File Setup
For each line of text in the game, we save it as a sub-object with language codes as keys. For example, if we wanted to save the start button in this format:

```
"BTN_START": {
    "EN": "Start Game",
    "RO_TEXT": "Începe Jocul"
}
```

Some sections have main and sub texts, in which case a sub-object would look like this:
```
"AREA_TEXT_0": {
    "MAIN": {
        "EN": "can you hear me?",
        "RO": "mă auzi?"
    },
    "SUB": {
        "EN": "Use WASD to move around.",
        "RO": "Folosește WASD pentru a te mișca."
    }
}
```

If you want to add more language codes, add them in the LANG section at the start of the JSON file. Use [standard ISO 639-1 language codes](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes). Please note that due to our formatter, these have to be exactly two letters long (the Series 1 table in the wikipedia article has all of the language codes we will use). Same goes for the text in each of the different text sections, they have to be exactly in the same format as in the example above. That is:
- Sub-object name in all caps (**DON'T** change this or add any)
  - Language code **in all caps** : "text that will appear in the game"

## Contributing
If you want to contribute to the translations, clone the repository to your computer and then use your favorite JSON editor (VS Code recommended) to edit the file. If you want, you can replace the `text.json` file in the StreamingAssets/Text folder of your build to be able to change the text in the game to the text in your JSON file. After you're done editing, submit a PR.

If you want to help test our game, please join our [Discord server](https://discord.gg/SmMf4ZC3eM)!

## Contributors
Thanks to all of our contributors who helped with the translations: 
[untilas](https://github.com/bendy1baldy2), who created the Russian translation.
