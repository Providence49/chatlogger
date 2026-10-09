# Providence Chatlogger

Turn a roleplay chat log into a clean, color-coded picture (PNG), with the spam filtered out. You can also put the chat on top of one of your own screenshots.

It is **one file**. There is nothing to install, no account, and no internet needed. Your chat is never uploaded anywhere. Everything happens on your own computer, inside your browser.

---

## Contents

1. [Install (2 minutes)](#1-install-2-minutes)
2. [Your first picture](#2-your-first-picture)
3. [What shows up and what colors mean](#3-what-shows-up-and-what-the-colors-mean)
4. [Fixing and styling lines directly on the picture](#4-fixing-and-styling-lines-directly-on-the-picture)
5. [Hiding names and words (blackout)](#5-hiding-names-and-words-blackout)
6. [Putting the chat on top of a screenshot](#6-putting-the-chat-on-top-of-a-screenshot)
7. [All the settings explained](#7-all-the-settings-explained)
8. [Saving your picture](#8-saving-your-picture)
9. [Typing the styling by hand (cheat sheet)](#9-typing-the-styling-by-hand-cheat-sheet)
10. [Something is wrong? Troubleshooting](#10-something-is-wrong-troubleshooting)

---

## 1. Install (2 minutes)

You do **not** install anything. You just download one file and open it.

### Step 1: Get the file

1. On this GitHub page, click the green **Code** button.
2. Click **Download ZIP**.
3. Find the downloaded `.zip` file (usually in your **Downloads** folder).
4. Right-click it and choose **Extract All…** (on a Mac, double-click it).
5. Open the folder that appears. You will see a file called **`providence-chatlogger.html`**.

> **Tip:** put that file somewhere you will remember, like your Desktop or Documents. You can also make a shortcut to it.

### Step 2: Open it

**Double-click `providence-chatlogger.html`.** It opens in your web browser and you will see the tool.

If it opens in something strange, or nothing happens: right-click the file → **Open with** → pick **Google Chrome**, **Microsoft Edge** or **Brave**.

> **Which browser?** Chrome, Edge and Brave work. Use one of those. (Firefox and Safari may work, but have not been tested.)

That's it. You are installed.

> **Bookmark it!** Once the page is open, you can bookmark it (press **Ctrl + D**) to open it quickly next time.

---

## 2. Your first picture

The left side is the menu. The right side shows your picture as you build it.

### Step 1: Put your chat in

You have two ways:

- **Paste it.** Copy your chat log text and paste it into the box under **1. Load a chatlog**.
- **Load a file.** Click **Choose file** and pick your `.txt` chat log, or drag the `.txt` file onto the page. You can pick several files at once and they will be joined together.

Your log should look something like this (a time in square brackets, then the line):

```
[23:55:26] Jane Doe says: So tonight... the bar.
[23:55:36] * John Smith flicks his arm up, checking his watch.
[23:55:47] John Smith says: Shouldn't be too long.
```

Right away you will see a picture appear on the right. By default it hides all the boring server messages (weather, "You don't have access to that command", etc.) and keeps the actual roleplay.

### Step 2: Pick which part you want

A whole play session has thousands of lines. You usually only want one scene.

Under **2. Line range** type the line number to start **From** and the number to stop **To**. The picture updates straight away. (Every line in your log gets a number, including the ones that are hidden, so just try numbers and look at the picture until it shows the right scene. Pasting a smaller piece of the log in the first place also works.)

### Step 3: Download it

Click the blue **Download PNG** button (top right). Your picture is saved to your normal **Downloads** folder.

You are done. Everything below is for making it look exactly how you want.

---

## 3. What shows up, and what the colors mean

Under **3. What to include** there are tick-boxes. Tick one to show that kind of line, untick to hide it.

| Kind of line | Example | Color | Shown by default? |
|---|---|---|---|
| Emotes (`/me`, `/do`) | `* John Smith waves.` | Purple | Yes |
| Says / shouts | `Jane Doe says: Hello` | White | Yes |
| Low / lower | `Jane Doe says [low]: Hello` | Light grey (lower = a bit darker) | Yes |
| Whispers | `Jane Doe whispers: Hello` | Orange | Yes |
| Phone / radio / car | `Jane Doe says (phone): Hello` | Yellow | Yes |
| Performance (mic) | `Jane Doe [Microphone]: la la la` | Yellow | Yes |
| Faction chat | `(( (64) Prospect John Smith: hey ))` | Dark green | No |
| OOC chat | `(( (60) Jane Doe: brb ))` | Grey | No |
| System / server messages | `[INFO] Your player ID is 5.` | Green | No |
| Session header | `[DATE: 22/AUG/2026 ...]` | Grey | No |

Also:

- A **pink `[!]`** at the start of a line means the line is aimed at your character (or someone you highlighted). Only the `[!]` is pink; the rest of the line keeps its normal color.
- **Show timestamps** adds the `[23:55:26]` time in front of each line.
- Dollar amounts (like `$300`) in **system messages** are shown in blue. You can turn that off in the Style section.

---

## 4. Fixing and styling lines directly on the picture

You can change anything right on the picture. **Click a line.** A little editor opens on top of it.

- Change the words however you like.
- Press **Enter** (or just click somewhere else) to apply.
- Press **Esc** to cancel.
- **Delete all the text in a line and press Enter to remove that line** from the picture.

Above the editor you will see a small bar with buttons. **Select some words** in the editor (drag over them with the mouse, or double-click one word), then click a button:

| Button | Shortcut | What it does |
|---|---|---|
| **✱ Emote** | Ctrl + E | Makes the selected words purple, like an emote (good for a quick action in the middle of speech) |
| **I Italic** | Ctrl + I | Makes the selected words italic |
| **█ Black out** | Ctrl + B | Covers the selected words with a black bar (see [section 5](#5-hiding-names-and-words-blackout)) |
| **Colored dots** | | Colors just the selected words (pick one of the 10 dots, or the box at the end for any color) |
| **✕** | | Removes the color from the selected words |

Click the same button again on the same words to **undo** it. You can keep the editor open and style several things before pressing Enter.

> **Note:** Emote and Italic are greyed out on lines that are already emotes and on system lines, because those don't use them. Black out and color work on every line.

**Important:** your edits only change the picture. They are **not** saved if you paste a new log or reload the page.

---

## 5. Hiding names and words (blackout)

Want to hide a real name or something private? Cover it with a black bar.

**The easy way:** click the line, select the word(s), click **█ Black out** (or press **Ctrl + B**).

**The typing way:** put a **`+`** on each side of what you want hidden, right in your chat text:

```
Jane Doe says: My real name is +John Smith+, don't tell anyone.
```

The picture shows a black bar where "John Smith" was. The `+` signs never show up in the picture.

Want to use a different symbol than `+`? Change it under **7. Black out text → Marker**.

---

## 6. Putting the chat on top of a screenshot

1. Scroll down the left menu to **6. Screenshot overlay**.
2. Click **Choose file** and pick a screenshot (or just drag an image onto the page).
3. Your chat now appears on top of the screenshot. The final picture has the **same size as your screenshot**.

Now place it:

- **Drag the chat box** on the picture to move it.
- **Drag a corner** (the little square handles on the dashed frame) to make the box bigger or smaller.
- Or use **Chat X / Chat Y** and **Box width / Box height**, or the **Top left / Top right / Bottom left / Bottom right** buttons.

By default **"Fit text to box"** is ticked: when you make the box bigger or smaller, the **text grows or shrinks automatically to fill it**. Untick it if you want to pick the text size yourself with the **Font size** setting.

Tips:

- Want just text with no dark box behind it? Click **Transparent** next to *Background* (in the Style section).
- Click **Remove screenshot** to go back to a plain chat picture.
- The chat box can't be dragged off the screenshot.
- Your screenshot is never uploaded, and is **not** remembered when you close the page.

---

## 7. All the settings explained

Everything is in the left menu. The picture updates instantly as you change things.

### 4. Your character

Type your character's name (exactly as it appears in the chat, for example `Jane Doe`).

- Your own says, low and lower lines are made **a bit lighter** than everyone else's, so you can tell which are yours.
- Your **phone lines turn white** (everyone else's stay yellow).
- Emotes and whispers are not touched.
- **Lighter by** controls how strong the difference is. 0 turns it off.

### 5. Style

| Setting | What it does |
|---|---|
| **Width** | How wide the picture is (in pixels) |
| **Font size** | How big the text is |
| **Outline** | Thickness of the black edge around the letters. 0 = no outline |
| **Line spacing** | The gap between lines (bigger = more air) |
| **Font** | Pick a typeface (Arial is the default) |
| **Background** | The color of the box behind the text |
| **Transparent** / **Solid** buttons | Jump the background to see-through or fully solid |
| **Opacity** | Slide from see-through to solid |
| **Highlight $ amounts in system messages** | Blue money amounts in system lines |
| **Drop exact duplicate consecutive lines** | If the same line appears twice in a row (this happens when copying logs), only keep one |

You can drag the sliders **or** type an exact number in the box next to each one.

### Reset

Click **Reset settings** (top of the menu) to put everything back to the starting values.

### Your settings are remembered

The tool remembers your settings (size, colors, font, which boxes are ticked, and so on) automatically and brings them back next time you open it in the same browser. It does **not** remember your chat text, your edits, or your screenshot.

---

## 8. Saving your picture

- **Download PNG** saves the picture to your Downloads folder. The file is named with the date and time, like `4.9.2026_16.28.44_chatlog.png`.
- **Copy image** copies the picture so you can paste it straight into Discord, Paint, etc. A message next to the button tells you if it worked. If it doesn't work in your browser, use Download PNG instead.

**Very long chats:** a picture can only be so tall. If your chat is too long, it is split into several pictures, and a note above the picture tells you. Download PNG then saves them one after another as `…_chatlog_part1.png`, `…_part2.png` and so on (your browser may ask if it is OK to download multiple files, say yes). Copy image can't copy a split chat, so either download, or choose a shorter line range. This doesn't happen when you use a screenshot, because the picture is then the size of the screenshot.

---

## 9. Typing the styling by hand (cheat sheet)

You never *have* to type these (the buttons do it for you), but you can write them in your chat text yourself.

| You type | You get |
|---|---|
| `*like this*` | Purple emote text (needs a `*` on both sides) |
| `/like this/` | *Italic* text (needs a `/` on both sides, at the start and end of a word) |
| `+like this+` | A black bar over the words |
| `{#FF5555:like this}` | The words in a color. The part after `#` is any color code (6 letters/numbers) |
| `[!]` at the start of a line | Pink `[!]` tag |

Things like dates (`9/11`), web links and commands like `/gps` are left alone, so a slash in the middle of normal text won't turn things italic.

---

## 10. Something is wrong? Troubleshooting

**The page is blank, or nothing happens.**
Open the file in Chrome, Edge or Brave (right-click the file → *Open with*).

**My picture says "nothing to show".**
No lines match. Check that your chat is pasted in, that the **From / To** line range covers some lines (click **Full log**), and that the right kinds of lines are ticked under *What to include*.

**Lines I expected are missing.**
Server/system lines, OOC and faction chat are hidden by default. Tick them under *What to include* if you want them. Also check the line range.

**The same line shows twice.**
Make sure *Drop exact duplicate consecutive lines* is ticked.

**My `*emote*` or `/italic/` doesn't work.**
The `*` and `/` must come in pairs on the same line (one at each end of the part you want styled). For italics, the slashes need to be at the edges of words.

**Copy image doesn't do anything.**
Some browsers block it. Use **Download PNG** instead.

**It downloaded lots of files.**
Your chat was long enough to be split. Use a shorter **From / To** range, or just keep all the parts.

**The text is tiny on my screenshot.**
Make the box bigger by dragging a corner (the text grows to fit), or untick *Fit text to box* and raise **Font size**.

**My settings were forgotten.**
Settings are stored by your browser. They are lost if you use a private/incognito window or clear your browser's site data.

**I messed everything up.**
Click **Reset settings** at the top of the left menu.

---

## Privacy

This tool runs entirely in your browser. It does not connect to the internet, send your chat anywhere, or collect anything about you. You can disconnect from the internet and it works the same.

---

*Providence Chatlogger is an independent tool and is not affiliated with GTA World, Rockstar Games, or any game server.*
