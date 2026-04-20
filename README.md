TC Calc
A fast, no-nonsense timecode calculator for the web. Built for video, audio post, and live production workflows.
https://stage-tools.github.io/TC-Calc/
---
Features
Add / subtract two timecodes, or add/subtract a raw number of frames or seconds to a timecode
Convert between timecode and total frames in both directions
Framerate support: 24, 25, 30, 50 fps
Live calculation — results update as you type
Click-to-copy on any result
Keyboard-friendly: auto-advance between HH/MM/SS/FF fields, arrow keys to increment/decrement
Swap A ↔ B with one click
Negative results are highlighted in red
Extra info for every result: total frames, seconds, minutes
Usage
Open the live demo — that's it. No install, no build step, no dependencies beyond Google Fonts.
Calc tab
Pick a framerate, enter `TC A`, choose `+` or `−`, then enter `B`. `B` can be:
TC — another timecode (e.g. compute duration between two TCs with `−`, or chain two durations with `+`)
Frames — a raw number of frames
Sec — a number of seconds, with decimals
Convert tab
Left: enter a timecode → get total frames
Right: enter total frames → get a timecode
Both conversions run live side by side.
Keyboard shortcuts
Key	Action
`↑` / `↓`	Increment / decrement the focused field
`Tab`	Move to next field
Type 2 digits	Auto-advance to next field
Click on result	Copy to clipboard
Running locally
Just open `index.html` in any modern browser. No server, no build.
```bash
git clone https://github.com/riccardonessi/tc-calc.git
cd tc-calc
# open index.html
```
Tech
Single-file HTML + vanilla JavaScript, no framework, no dependencies.
Fonts: Share Tech Mono and Barlow Condensed from Google Fonts.
Notes
Non-drop-frame math only. 29.97 DF / 59.94 DF are not currently supported.
Results wrap at 99:59:59:FF (HH field caps at 99).
License
MIT
---
Made by Riccardo Nessi
