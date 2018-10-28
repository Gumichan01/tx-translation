# Translation data (i18n) - Target Xplosion #

This repository contains every translation data of
[Target Xplosion](https://github.com/Gumichan01/target-xplosion).

Syntax:

    tx_<language>.po


## How to use it ##

You can use the *.pot* file to generate the *.po* file.

    msginit --no-translator --locale=<language> --input=tx.pot --output=tx_<language>.po

Now you can translate the strings.
After that, you must generate the *.mo* file.

    msgfmt --statistics tx_<language>.po -o tx_<language>.mo


Copy the *.mo* file in the `config/` directory of [the game](https://github.com/Gumichan01/target-xplosion).

## contribution ##

Internationalization and Localization are supported by Target Xplosion.
You don't need to select a language, it is detected by the game.
However, I started to create this repository, so people can start to translate
the game in several languages.
