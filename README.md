# KeyCheck

A simple browser-based keyboard tester. Press keys and see right away which ones work.

> **Status: test app.** KeyCheck is an experimental project built for testing and learning. Features, design, and behavior are **subject to update** and may change without notice.

## Features

- On-screen keyboard with the main keys, function row, navigation cluster, arrow keys, and numpad
- Keys glow yellow while held down
- Keys turn mint green once they have registered, so untested keys are easy to spot
- Live display of the last key pressed, including its `code` and `keyCode`
- Short history of recent key presses
- Progress ring showing how many keys are working
- "Start over" button to reset the test
- Follows your system light or dark mode

## Known limitations

- Keys are matched by physical position (`KeyboardEvent.code`), so labels follow a standard US layout even if your keyboard layout is different.
- The **Fn** key is handled by the keyboard hardware and cannot be detected by a browser.
- Some keys, such as **Print Screen** or the **Windows** key, may be captured by the operating system before the browser sees them.
- Some browser or system shortcuts (for example `Ctrl+W` or `Alt+F4`) cannot be blocked and may still trigger.
- Built for physical keyboards on desktop or laptop. It is not meant for touch screens.

## Tech

- Single self-contained HTML file with plain HTML, CSS, and JavaScript
- No frameworks or build tools
- Uses the [Sora](https://fonts.google.com/specimen/Sora) font from Google Fonts, with a system font fallback

## Disclaimer

KeyCheck is provided as is, as a test app. It may contain bugs and is not intended as a professional hardware diagnostic tool.