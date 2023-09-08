# Uninstalling Applications on macOS

This guide provides different methods for uninstalling applications on macOS.

## Table of Contents
1. [Method 1: Drag-and-Drop](#method-1-drag-and-drop)
2. [Method 2: Using Launchpad](#method-2-using-launchpad)
3. [Method 3: Using Terminal](#method-3-using-terminal)
4. [Cleaning Up Leftover Files](#cleaning-up-leftover-files)

---

## Method 1: Drag-and-Drop

For Apps from the Applications Folder:

1. **Open the Applications Folder**: Open Finder and then select `Applications` from the sidebar, or use the shortcut `Shift + Command + A`.

2. **Locate the Application**: Find the application you want to uninstall.

3. **Move to Trash**: Drag the application to the Trash located in your Dock.

4. **Empty the Trash**: Right-click on the Trash icon and select `Empty Trash`.

---

## Method 2: Using Launchpad

For Apps Downloaded from the App Store:

1. **Open Launchpad**: Click its icon in the Dock or use a trackpad gesture (pinch the thumb and three fingers together).

2. **Locate the Application**: Find the application you wish to uninstall.

3. **Initiate Uninstallation**: Click and hold the application’s icon until it starts to wiggle.

4. **Confirm Uninstallation**: Click on the `X` that appears on the top-left corner of the application icon and confirm.

---

## Method 3: Using Terminal

**Warning: For Advanced Users. Be extremely careful with the commands you enter.**

1. **Open Terminal**: You can find the Terminal app in the `Utilities` folder within the `Applications` folder.

2. **Run the Uninstall Command**: Use the `rm -rf` command to remove the application. 

    ```bash
    sudo rm -rf /Applications/[ApplicationName].app/
    ```

    Replace `[ApplicationName]` with the name of the application. **This will delete files without any confirmation.**

---

## Cleaning Up Leftover Files

After uninstalling, some leftover files may remain.

1. **Open Finder**: Just click on the Finder icon.

2. **Navigate to Folder**: Click `Go` in the menu bar, then select `Go to Folder` or use the shortcut `Shift + Command + G`.

3. **Type the Path**: Type `~/Library/Preferences/` or `~/Library/Application Support/`.

4. **Search and Remove**: Search for folders or files related to the application you’ve uninstalled and move them to the Trash.

---


