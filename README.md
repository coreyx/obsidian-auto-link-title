## Obsidian Auto Link Title
![Auto linking example](auto-link-title.gif)

### Installing With BRAT
This fork can be installed with the [BRAT](https://github.com/TfTHacker/obsidian42-brat) (Beta Reviewers Auto-update Tool) plugin:

1. Install **BRAT** from Obsidian's Community Plugins browser and enable it.
2. Open the command palette and run **BRAT: Plugins: Add a beta plugin for testing**.
3. Enter `https://github.com/coreyx/obsidian-auto-link-title` as the repository.
4. Choose the latest version (or leave it as the default) and select **Add Plugin**.
5. If you already have the official Auto Link Title installed, BRAT replaces it with this fork, since both use the same plugin ID. Otherwise, enable **Auto Link Title** in **Settings → Community plugins**.

BRAT checks for updates on startup, or you can run **BRAT: Check for updates to all beta plugins** to update manually.

### Automatically Title New Links
This plugin automatically fetches the webpage to extract link titles when they're pasted, creating a markdown link with the correct title set.

#### For example:

When pasting `https://github.com/zolrath/obsidian-auto-link-title` the plugin fetches the page and retrieves the title, resulting in a paste of: `[zolrath/obsidian-auto-link-title: Automatically fetch the titles of pasted links](https://github.com/zolrath/obsidian-auto-link-title)`

### Add Titles To Existing Raw URLs
Additionally, using `ctrl-shift-e` (Windows) or `cmd-shift-e` (OS X) you can enhance an existing raw link to a markdown formatted link with the proper title.

If your text cursor is within the url `https://github.com/zolrath/obsidian-auto-link-title` pressing `ctrl-shift-e` or `cmd-shift-e` converts the text to `[zolrath/obsidian-auto-link-title: Automatically fetch the titles of pasted links](https://github.com/zolrath/obsidian-auto-link-title)`

### Overwrite Titles Of Existing Markdown Links
Additionally, using `ctrl-shift-e` (Windows) or `cmd-shift-e` (OS X) you can overwrite an existing title of a markdown link with the fetched title from the url.

If your text cursor is within `[some plugin](https://github.com/zolrath/obsidian-auto-link-title)` pressing `ctrl+shift+e` fetches the sites title and replaces it, resulting in `[zolrath/obsidian-auto-link-title: Automatically fetch the titles of pasted links](https://github.com/zolrath/obsidian-auto-link-title)`

### Mobile Pasting
In order to paste the URL ensure you perform the `Tap and Hold -> Paste` action to paste the URL into your document.

#### Gboard
Google's [Gboard](https://play.google.com/store/apps/details?id=com.google.android.inputmethod.latin&hl=en_US&gl=US) keyboard has a Clipboard helper shortcut above the keyboard to quickly paste.
Due to the implementation of that feature, it does not trigger the `paste` event, preventing this plugin from interacting with the text.
