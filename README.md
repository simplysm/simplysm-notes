# Simplysm Notes

English | [한국어](README.ko.md)

A Windows note app that uses a GitHub repo as its storage. Your notes are stored only in your own GitHub repo. The app keeps a local clone of that repo and automatically commits and pushes your edits.

> This repository is for **installer releases** and **feedback**. The source code is not public.

## What it does

- **Your notes live only in your GitHub repo.** There is no service to sign up for and no server in between. Without the app, the notes still read as-is on the GitHub website.
- **No need to think about saving or syncing.** Edits are saved as you type, and the app pushes them to GitHub and pulls changes on its own. Changes made on another PC come in automatically. It works offline and pushes once you are back online.
- **When the same spot is edited in two places, you choose.** The app never silently drops one side; you see both sides in a merge view and decide.
- **Edit the Markdown source as-is.** What you see is the file content, so merely opening a note never changes the file. Headings, lists, tables and code blocks (colored per language) are highlighted, tables are shown with aligned columns, and rows and columns move with shortcuts.
- **Link notes to each other.** Insert links with `[[` autocomplete or by dragging from the tree, and open them with Ctrl+click. When you move or rename a note or folder, links pointing to it are updated too.
- **Attach files and images to notes.** Drop or paste them to attach; images show inline in the note.
- **Find any note at once.** One search box finds titles and content across all connected notebooks as you type.
- **See and restore past versions.** View the change history of each note or folder, compare what changed, and restore only the notes you pick.
- **Share a folder with your team.** The chosen folder is automatically replicated to another repo, and recipients open that repo as read-only. Replication keeps running on GitHub even when the app is off.
- **A terminal is built in.** Open a shell right in the notes folder and work on notes with a coding agent such as Claude Code; the changes show up in the app.
- **Stays in the notification area.** Sync keeps running after you close the window, and the app starts with Windows (you can turn this off in Settings).
- The display language can be English or 한국어 (Korean).

## Getting started

1. Download the installer from "Download" below and run it.
2. **Sign in with GitHub.** Paste the code the app shows into the GitHub page and approve.
3. **Connect a repo to use as a notebook.** Pick one from your repo list, or enter `owner/repo` or a URL. Repos you cannot write to open as read-only.

## Download

Download `notes-win32-x64-<version>.exe` from [Releases](../../releases/latest) and run it.

- Windows 10/11 (64-bit)
- No administrator rights needed. It installs into your user folder.
- git is bundled with the app, so you do not need to install it separately.

## Blue warning during installation (SmartScreen)

This installer is **not code-signed yet.** So the first time you run it, Windows shows a blue "Windows protected your PC" window.

1. Click **More info**.
2. Click **Run anyway**.

Code signing will be added as the number of users grows.

## Updates

The app downloads new versions on its own, and when one is ready an **Install update** button appears at the top of the window. It restarts and applies the update only when you click that button — it never interrupts your work.

## Where your data is

- Notes: the connected GitHub repo, and its local clone folder (default `Documents\Simplysm Notes\<owner>\<repo>`)
- App settings: `%APPDATA%\Simplysm Notes`

Uninstalling the app leaves your notes folder in place.

## Bug reports · Feature requests

Please leave them in [Issues](../../issues). Bug reports, feature requests, and questions about using the app are all welcome.
