# Lambe

Lambe is a graphical tool for creating and using Tengwar modes, transcribing text and adjusting glyph placement. Created and developed by **André I. Ben**, **Lambe Labs**.

## Download the ready-to-run apps

- **[Windows x64: download the complete app folder](https://github.com/Awarrz/Lambe/releases/download/v0.9.6/Lambe-0.9.6-Windows-x64.zip)** (ZIP). Extract all files, open the `Lambe` folder and run `Lambe.exe`. Keep the included DLLs, `data` and `modes` folders together.
- **[Android: download the installable APK](https://github.com/Awarrz/Lambe/releases/download/v0.9.6/Lambe-0.9.6-Android.apk)**. Open the APK on your Android device to install Lambe.

Both downloads are already compiled and include fonts and modes. No Flutter SDK or compilation is required.

GitHub also shows automatic **Source code (zip)** and **Source code (tar.gz)** archives. Those contain this repository’s documentation and shared files. For the apps, use the Windows ZIP or Android APK linked above.

## Documentation

- [Illustrated user guide (PDF)](docs/Lambe_User_Guide_v0.9.6_Illustrated.pdf): using Lambe and reading Tengwar in English, Quenya and Sindarin.
- [Illustrated JSON mode reference (PDF)](docs/Lambe_JSON_Mode_Reference_Illustrated.pdf): editing mode definitions, associations, marks and contextual rules.

The editable [Arabic Arabizi mode](modes/arabic-romanized-lambe.json) is already included in both apps.

## Features

- Create and duplicate language modes through graphical associations and contextual rules.
- Choose a tengwa, a tehta or a combination as a rule's output.
- Move individual tengwar and tehtar, including independent adjustments and combined glyph work.
- Preserve newlines and empty lines; export the finished result as a PNG.
- Choose ordinary or Tengwar numerals, with separate handling for Arabizi digit letters.
- Use the font studio and save fonts.

Lambe transcribes your input into Tengwar; it does not translate between languages. This is an open alpha. Review your result and send practical feedback through [Issues](https://github.com/Awarrz/Lambe/issues).

## Modes and saved work

English, Romanised Hebrew, Quenya, Sindarin, Beleriand, German orthographic and Arabic Arabizi are supplied. Inputs and previews start blank. On Windows, saved modes use the `modes` directory beside the app when writable, with an app-data fallback. Android keeps modes in its own app storage. Export important custom modes before moving, replacing or uninstalling an installation.

## Credits

See [credits](CREDITS.md) and [third-party notices](licenses/THIRD_PARTY_NOTICES.txt). Fonts retain their accompanying SIL Open Font License. Arabic consonant assignments follow Gabriel McGovern's 2016 chart, with Lambe's Arabizi input aliases.

This repository contains downloads, documentation and shared mode definitions. The development project is not required by users.

