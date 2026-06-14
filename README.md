# IslandFerry

IslandFerry is a productivity tool for macOS that combines a file staging area and a clipboard manager into a lightweight, always-available workspace.

## Why IslandFerry

In day-to-day work, a lot of things just need a temporary place to stay before you use them again.

For example:

- You want to drag several files into a chat window, but you have not gathered them all yet
- You just copied a piece of text, a link, or an image, and need to paste it again later
- You want to temporarily collect a few materials before organizing them together
- You frequently move files and content between multiple apps

IslandFerry is built for exactly these high-frequency, fragmented, cross-app workflows.

It turns the top of your screen into an always-ready productivity hub:

- `Shelf` on the left for temporarily storing files and folders
- `Clipboard` on the right for saving and managing copied content

## Usage

### 1. File Shelf: Make Drag-and-Drop Smoother
- Drag files and folders in directly
- Drag them back out anytime to Finder (copy), chat windows, or other apps
- Hold the `Cmd` key and start dragging to move the original file to another Finder location
- Quickly open the original file or reveal it in Finder
- Open folder items in Terminal with one click

Great for scenarios like:

- Organizing a batch of attachments before sending them
- Temporarily gathering multiple assets before distributing them
- Parking "in-progress" project files in a fixed spot while you work

### 2. Clipboard Management: Actually Keep What You Copy

- Enable auto collection in `Settings` to automatically save content whenever you copy
- Or capture only with the dedicated shortcut `Control + X` to avoid unnecessary interruptions
- Rename items, mark them as important, search, filter, and delete
- Clear non-important items while keeping the truly valuable snippets
- Set ignore rules for specific apps so sensitive or irrelevant copied content is not collected

### We’re continuously improving IslandFerry and adding new features. Stay tuned, and we’ll share the latest updates with you as soon as they’re released.

## Installation

**System Requirements:**

- macOS **14 Sonoma** or later
- Apple Silicon or Intel Mac

***

### Option 1: Download and Install Manually

<a href="https://github.com/JasperQin-ky/island-ferry-releases/releases/latest/download/IslandFerry-v0.4.0.dmg" target="_self"><img width="200" src="https://github.com/user-attachments/assets/e3179be1-8416-4b8a-b417-743e1ecc67d6" alt="Download for macOS" /></a>

Once downloaded, open the `.dmg` and move **IslandFerry** to your `/Applications` folder.

> \[!IMPORTANT]
> We don't have an Apple Developer account (yet 👀), so macOS will warn you that IslandFerry is from an unidentified developer on first launch. This is expected behavior.
>
> You'll need to bypass this before the app will open. You only need to do this once. Use one of the methods below.

***

#### Recommended: Terminal (Always Works)

This is the quickest and easiest method. It only requires a single command and works consistently for all users. System Settings can sometimes fail and won't work for non-admin users.

After moving IslandFerry to your Applications folder, run:

```bash
xattr -dr com.apple.quarantine /Applications/IslandFerry.app
```

Then open the app normally.

***

#### Alternative: System Settings

> \[!NOTE]
> This method doesn't work for all users. If this doesn't work, use the Terminal method above.

1. Try to open the app — you'll see a security warning.
2. Click **OK** to dismiss it.
3. Open **System Settings** > **Privacy & Security**.
4. Scroll to the bottom and click **Open Anyway** next to the IslandFerry warning.
5. Confirm if prompted.