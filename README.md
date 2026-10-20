<p align="center">
  <img src="icon.png" alt="GibrishFixer icon" width="120">
</p>

<h1 align="center">GibrishFixer</h1>

<p align="center">
  <em>Typed Hebrew when you meant English, or English when you meant Hebrew?<br>Fix it in one keypress.</em>
</p>

<p align="center">
  <a href="https://github.com/snir-hoffman/GibrishFixer/releases"><strong>Download for Windows</strong></a>
  &nbsp;·&nbsp;
  <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Space</kbd>
</p>

---

## The problem

You are writing in one language, but your keyboard is still set to the other. The letters come out wrong, even though the keys you pressed were right. The word is still there, just in the wrong alphabet.

```
You typed:  יקךךם   →   Fixed:  hello
```

## What it does

GibrishFixer lives in your system tray. When you press **Ctrl + Shift + Space**, it:

1. **Finds the text.** It uses your selection, or the word just before the cursor if nothing is selected.
2. **Converts it.** Each key is mapped to the same key on the other keyboard layout, keeping capitals and punctuation.
3. **Switches the language.** Your typing language changes to the one the text now uses, so you can keep typing.

It doesn't guess the language. You decide when to fix, and it converts exactly what you selected.

## Features

- **Any installed language.** Works with every keyboard layout installed in Windows.
- **You stay in control.** Nothing changes until you press the hotkey.
- **Choose the target.** Pick which language to convert to, or let it use the other one.
- **Settings window.** Choose languages, start with Windows, and turn debug logging on or off.
- **Lightweight.** Runs quietly in the system tray.
- **Private.** Text is only read when you press the hotkey, and it is never sent anywhere.

## Get started

1. Download **GibrishFixer.exe** from the [releases page](https://github.com/snir-hoffman/GibrishFixer/releases) and run it.
2. Windows may show a *"Windows protected your PC"* warning, because the app is not signed with a commercial certificate. Click **More info**, then **Run anyway**.
3. Select mistyped text (or place the cursor after a word) and press **Ctrl + Shift + Space**.

Right-click the tray icon for the menu and settings.

## Requirements

- Windows 10 or 11
- Keyboard layouts installed in Windows (Settings → Time & language → Language & region)

## Build from source

```
pip install -r requirements.txt
pyinstaller --noconfirm --onefile --noconsole --name GibrishFixer --icon icon.ico --add-data "icon.png;." app.py
```

The exe is written to `dist\GibrishFixer.exe`.

---

<p align="center">
  <sub>Made for everyone who switches between Hebrew and English.</sub>
</p>
