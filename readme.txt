Here's a Q&A!

Q: How are the assets organized?
A: Every folder inside "assets/" is copied to the game with the same name:
assets/preload/ - menus, title screen, UI, menu sounds and menu music
assets/shared/ - gameplay images (characters, icons, notes, ratings in images/ui), stages, weeks, data, music and sounds
assets/week1/ ... assets/weekend1/ - files that only one week uses
assets/songs/ - Inst and Voices for every song
assets/videos/ - cutscenes
assets/fonts/ - fonts
assets/embed/ - files embedded inside the executable

Q: Where does the game look for a file?
A: First in the current week folder, then in "assets/shared/", then in "assets/preload/".
Old paths still work: images/menuBG.png is found at images/menus/menuBG.png (see source/funkin/assets/AssetAliases.hx).

Q: Where should I put my charts?
A: "assets/shared/data/your-song-name/".

Q: Where should I put my songs?
A: "assets/songs/your-song-name/" with Inst.ogg and Voices.ogg.

Q: Where should my week files go?
A: Create a folder like "assets/weekpsychic/" next to "assets/week1/", it will be packaged automatically.

Q: I don't want base game assets in my mod! What should I do??
A: Remove "BASE_GAME_FILES" from project.hxp. Every base game file is listed in "project/assets/base_game.txt" and gets skipped when it is off.

Q: What about translations and the title screen secrets?
A: They live inside "assets/shared/" too and are listed in "project/assets/translations.txt" and "project/assets/secrets.txt",
turning off "TRANSLATIONS_ALLOWED" or "TITLE_SCREEN_EASTER_EGG" skips them.
