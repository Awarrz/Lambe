# Lambe

Lambe is a graphical tool for creating and using Tengwar modes, transcribing text and adjusting glyph placement. Created and developed by **André I. Ben**, **Lambe Labs**.

## Download

Open [Releases](https://github.com/Awarrz/Lambe/releases) and choose the Windows ZIP or Android APK. Extract the entire Windows ZIP and open `Lambe.exe`. Keep its DLLs, `data` and `modes` folders together. Install the APK on Android. Flutter is not required to run either download.

The release also contains the [user guide](docs/USER-GUIDE.md) and an editable [Arabic Arabizi mode](modes/arabic-romanized-lambe.json). The mode is already included in both apps.

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
