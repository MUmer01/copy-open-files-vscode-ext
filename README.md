# Context Copier

## Overview

Context Copier is a powerful VS Code extension designed to streamline your workflow when you need to share code. It eliminates the tedious process of manually copying and pasting files one by one.

Whether you're crafting a detailed prompt for an AI assistant like ChatGPT/Claude, preparing a code review, or creating documentation, Context Copier lets you grab the path and content of one or multiple files in a single, effortless action.

## Core Features

- **Dual Output Modes:** Choose to either copy content directly to your **clipboard** or **combine it into a new, temporary file** for review and editing.
- **Flexible Selection:** Grab content from a single file, a multi-selection of files in the Explorer, the currently active file, or all open tabs at once.
- **Intuitive Triggers:** Access all features directly from the **File Explorer context menu**, the **Editor Tab context menu**, a **keyboard shortcut**, or the Command Palette.
- **Intelligent Path Handling:** Automatically includes the relative file path for each file, preserving project structure and context.
- **Handles Unsaved Files:** Works perfectly with new, unsaved files (e.g., `Untitled-1`), ensuring no part of your work is left behind.

## How to Use

Context Copier integrates seamlessly into your workflow. You can trigger its commands in three main ways:

#### 1. From the File Explorer

Right-click on one or more files in the Explorer sidebar to quickly copy their content to your clipboard.

- **Copy Path & Content (Context Copier):** Copies the selected file(s) to the clipboard.

#### 2. From an Editor Tab

Right-click on any open file tab at the top of the editor to access all the extension's features. This is the most powerful entry point.

- **Copy Path & Content of This Tab:** Copies just the right-clicked tab's content to the clipboard.
- **Copy Path & Content of All Open Tabs:** Copies all open tabs to the clipboard.
- **Combine This Tab into New File:** Opens the content of the right-clicked tab in a new, unsaved document.
- **Combine All Open Tabs into New File:** Opens the content of all open tabs in a new, unsaved document.

#### 3. From the Active Editor

Use a keyboard shortcut or the Command Palette for the fastest access.

- **Keyboard Shortcut:** Press `Ctrl+Alt+C` (`Cmd+Alt+C` on Mac) to copy the currently active file to the clipboard.
- **Command Palette:** Press `Ctrl+Shift+P` (`Cmd+Shift+P` on Mac), type "Context Copier", and choose the desired command.

## Example Output

Let's say you have two files open and you use the "Copy All Open Tabs" command. The text copied to your clipboard will look like this, with a clear separator between files:

```
// File 1: /src/main.js

import { helper } from './utils/helper.js';

function main() {
    console.log(helper());
}

main();

---

// File 2: /src/utils/helper.js

export function helper() {
    return "Hello from helper!";
}
```

You can now easily paste this entire block of context into an AI assistant.

## Requirements

No special requirements or dependencies.

## Known Issues

Currently none. Please report any issues you encounter on the GitHub repository.

## Release Notes

### 1.0.0

Initial release of **Context Copier**.

- Introduced 6 commands for flexible content gathering.
- Added dual output modes: "Copy to Clipboard" and "Combine into New File".
- Enabled triggers from the File Explorer, Editor Tabs, and Keyboard Shortcuts.
- Full support for saved and unsaved files.

---

**Enjoy using Context Copier to streamline your interactions with AI and improve your coding workflow!**
