# Global Legends: test builds

This page has the downloads for **Global Legends**, a game made from the novel *Global Legends, Season 31, Book One*. It's a private family project and isn't for sale. The builds are here so the author can play them and send notes back.

There is **no source code** in this repository, only the downloads (under **Releases**, on the right) and this page.

**Newest build:** <https://github.com/Southeastern-Renovation/global-legends-builds/releases/latest>

---

## What's in a build

**Book One, Levels 0 to 12.** Every chapter of the book has a level, from the facility prologue to the end of Book One. It's an early test build: the story, the places and the fights are all in, but plenty is rough. The release notes for each build list what changed and what's known to be broken.

| Download | For |
|---|---|
| `GlobalLegends-Mac-<version>.zip` | A Mac with an Apple chip (M1 or newer), macOS 14 Sonoma or newer |
| `GlobalLegends-Windows-<version>.zip` | A Windows 10/11 PC with a gaming graphics card (only when a Windows build is posted) |
| `….zip.part-aa`, `….zip.part-ab`, … | A build over 2 GB, split in pieces. Download every piece, then follow `HOW-TO-JOIN-Mac.txt` or `HOW-TO-JOIN-Windows.txt` |
| `SHA256SUMS-*.txt` | Fingerprints to check the download wasn't damaged (optional) |

---

## Install on a Mac

1. Download the Mac zip from the newest release (no GitHub account needed). If it comes in pieces, join them first with `HOW-TO-JOIN-Mac.txt`. Double-click the zip. You get **Global Legends.app**.
2. Drag **Global Legends.app** into **Applications**.
3. **The first time only,** the Mac blocks the game, because it isn't from the App Store and isn't registered with Apple. That's expected for a home-made game.
   - **macOS 15 (Sequoia) or newer:** double-click the game. When it says Apple couldn't check it, click **Done**. Open **System Settings → Privacy & Security**, scroll down to the message about "Global Legends", click **Open Anyway**, and enter your password.
   - **macOS 14 (Sonoma):** right-click (or Control-click) the game, choose **Open**, then click **Open** again.
4. After that it opens with a normal double-click.

If neither works, open Terminal and paste this line, then double-click the game again:

```
xattr -dr com.apple.quarantine "/Applications/Global Legends.app"
```

**Updates:** download the new zip and replace the old app. Saved games are kept somewhere else, so they survive:
`~/Library/Containers/com.globallegends.GlobalLegends/Data/Library/Application Support/Epic/GlobalLegends/Saved/SaveGames`

## Install on Windows

1. Download the Windows zip. If it comes in pieces, join them first with `HOW-TO-JOIN-Windows.txt`. Right-click the zip, choose **Properties**, tick **Unblock** if it's there, click **OK**.
2. Right-click the zip, choose **Extract All…**, and pick a short folder such as `C:\Games\GlobalLegends`. Don't run the game from inside the zip.
3. Double-click **GlobalLegends.exe**. If a blue "Windows protected your PC" box appears, click **More info**, then **Run anyway**. If a "Microsoft Visual C++" installer appears, let it install.

Saved games: `C:\Users\<you>\AppData\Local\GlobalLegends\Saved\SaveGames`

---

## Starting a game

On the title screen:

- **New Game** starts at Level 0 and asks for a difficulty. **Normal** is challenging. **Legend** has smarter enemies, no map in dungeons and stronger poison. **Permadeath** gives you one life.
- **Continue** goes back to your last checkpoint. The game saves by itself at checkpoints, and there's no save button.
- **Chapters** starts any level from its beginning, with the gear and character level it normally opens with, so you can jump straight to the part you want to check. A level shown greyed out with "(play from the start)" can't start on its own yet; reach it by playing through. **Starting a chapter replaces your current Normal game.**
- **Codex** shows everything you've learned so far.

## Controls

| Key | What it does |
|---|---|
| **W A S D** | Walk |
| **Mouse** | Look around and turn |
| **Shift** (hold) | Hurry |
| **E** | Talk, open, pick up, use |
| **Left mouse button** | Attack |
| **Right mouse button** (hold) | Block |
| **F** | Bash (a shoving blow) |
| **Q** | Eat (travel biscuits first, then bread) |
| **Space**, **Enter** or **left click** | Continue a conversation |
| **1 2 3 4** | Choose a reply |
| **Y / N** | Accept or decline a party invite |
| **Tab** | Game menu: Status, Inventory, Map, Codex |
| **M** | Map |
| **C** | Codex |
| **Esc** | Pause menu (it has a **Controls** page). Esc also closes any open window. |
| **Alt+Enter** or **F11** (Mac: **Option+Return**) | Full screen or window |

There's no jump. At a forge, strike with **Space**, **E** or **left click**, and press **Esc** to step away.

Puzzle keys are shown on screen when needed (e.g. the Level 9 ring lever).

**Controller (partial):** left stick moves, right trigger attacks, left trigger blocks, right bumper bashes, A continues a conversation, Start pauses, Back opens the game menu. v0.1: Interact is keyboard E only. The right stick doesn't turn the camera yet.

---

## Sending notes

Your notes decide what gets fixed first. The most useful thing to say is where the game doesn't feel like the book. Copy this into a text or an email to Jared and fill it in as you play. One line per question is plenty.

```
GLOBAL LEGENDS - TESTER NOTES
Build (the release name, e.g. v0.1-2026-10-01):
Mac or Windows? (Windows: graphics card from Start > "dxdiag" > Display tab > Name):
Did it run smoothly? (smooth / a bit choppy / very choppy):
Difficulty you played (Normal / Legend / Permadeath):

----------------------------------------------------------------
LEVEL __ : ________________________   (copy this block for each level)

1. Did it feel like the book?  (yes / mostly / not really)
   Why:

2. What's missing? (a moment, a line, a character, a place, a feeling)

3. What's wrong? (someone acting out of character, wrong order,
   wrong place, wrong words)

4. Difficulty, 1 to 5:   1 = too easy   3 = about right   5 = too hard
   Score:
   Where was it hardest / most boring?

5. Bugs (anything broken). For each one:
   - What happened:
   - What you were doing just before (steps, in order):
       1.
       2.
       3.
   - Where (level, and roughly where in it):
   - Does it happen again if you try the same thing? (yes / no / didn't try)
   - Screenshot? (Mac: Shift+Cmd+4. Windows: Windows key + Shift + S)

6. Best moment in this level:

----------------------------------------------------------------
OVERALL
- Which character is furthest from how you imagined them?
- Anything from the book that must be in the game and isn't?
- Anything the game added that you don't like?
```

**If the game crashes,** write down what you were doing and send Jared the newest crash folder:
- Mac: `~/Library/Logs/DiagnosticReports` (files starting with "GlobalLegends")
- Windows: `C:\Users\<you>\AppData\Local\GlobalLegends\Saved\Crashes`

---

*Personal use only. Not for sale or redistribution.*
