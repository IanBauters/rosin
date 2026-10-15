# Rosin

Falling-notes practice videos for cello. Open a MIDI or MusicXML file and Rosin shows the music three ways at once:

- **Sheet music** scrolling along the top, engraved from your score
- **A note highway** with one lane per string (A, D, G, C, as you see them holding the cello), each note marked with the finger to use
- **A fingerboard** showing the hand position and where every finger goes

**[Open Rosin](https://ianbauters.github.io/rosin/)**

## What it does

- Opens `.mid`, `.midi`, `.xml`, `.musicxml` and `.mxl` files, or plays the built-in sample (Bach, Prelude from Cello Suite No. 1)
- Suggests a fingering for every note: string, finger and position, keeping shifts and string crossings low. Fingerings and strings written in a MusicXML file are used as they are.
- Shows upcoming shifts on the highway, and on the fingerboard the fingers that stay down behind the one playing
- **Watch** mode, or **Play along** with the keyboard (D F J K) or by tapping the rings, with score and streak
- Set the speed to any percentage from 25% to 200% without changing the pitch; the tempo is shown as quarter notes per minute (for example ♩ = 90), next to the original tempo. 100% is the tempo written in the file; a file without a tempo plays at ♩ = 120
- Note names in do-re-mi or C-D-E
- Records a 1080p video with sound and lets you download it (MP4 or WebM, depending on the browser)
- Light, dark or automatic theme for the page

Everything runs in your browser. Your files are not uploaded anywhere.

## Notes and limits

- The fingering is a suggestion from a search that keeps the hand movement low. It is a guide, not a teacher's edition.
- MIDI files have no notation of their own, so Rosin writes a clean score from the notes. Slurs and articulations only appear when they are in a MusicXML file.
- Repeat signs in MusicXML are drawn but not followed during playback: the music plays straight through once.
- The sheet music needs an internet connection the first time the page opens (the notation engine loads from a CDN). Without it, Rosin falls back to a simple staff.
- Recording works best in a recent Chrome, Edge, Firefox or Safari on a computer. Keep the tab in front while it records.

## Credits

- **Cello sound**: notes rendered from the Musyng Kite soundfont, via [gleitz/midi-js-soundfonts](https://github.com/gleitz/midi-js-soundfonts), licensed [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). The sound data embedded in `index.html` stays under that license.
- **Sheet music**: [OpenSheetMusicDisplay](https://github.com/opensheetmusicdisplay/opensheetmusicdisplay) (BSD-3-Clause), loaded from jsDelivr
- **.mxl files**: [JSZip](https://github.com/Stuk/jszip) (MIT), loaded from cdnjs
- **Fonts**: Saira, Saira Condensed and Noto Music from Google Fonts (SIL Open Font License)
- Inspired by [TileDropper](https://tiledropper.github.io/TileDropper/)

## License

The code is released under the MIT License, see [LICENSE](LICENSE). The embedded cello sound data is CC BY-SA 3.0 as noted above.
