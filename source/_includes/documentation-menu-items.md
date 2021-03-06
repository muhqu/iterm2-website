#### iTerm > Secure Keyboard Entry
When this is enabled, the operating system will prevent other programs running on your computer from being able to see what you are typing. If you're concerned that untrusted programs might try to steal your passwords, you can turn this on, but it may disable global hotkeys in other programs.
#### Shell > New Tab with Current Profile
This creates a new tab using the same profile as the current session rather than the default profile.
#### Shell > New Window/Tab
This creates a new window or tab with the default profile. If the current session is a tmux integration session, then the new window or tab will be a tmux window.
#### Shell > Split Vertically/Horizontally
These menu items allow you to divide a tab into two or more split panes. The panes can be adjusted by dragging the line that divides them. They will use the default profile.
#### Shell > Split Vertically/Horizontally with Current Profile
These menu items allow you to divide a tab into two or more split panes. The panes can be adjusted by dragging the line that divides them. They will use the profile of the current session.
#### Shell > Broadcast Input > ...
These options allow you to send keyboard input to more than one session.
#### Shell > Run/Stop Coprocess
Allows you to start and stop a coprocess linked to the current session. Learn more about coprocesses.
#### Shell > tmux > ...
These commands let you interact with the tmux integration. The tmux dashboard is a view that lets you see all your tmux sessions and windows at a glance, adjust which are visible, rename them, and change the current tmux session.
#### Shell > Log > Start/Stop
Logging saves all input received in a session to a file on disk.
#### Edit > Paste Special > Paste Escaping Special Characters
"Paste Escaping Special Characters" pastes the current string in the clipboard, but places a backslash before spaces and backslashes.
#### Edit > Paste Slowly
"Paste Slowly" pastes the current string in the clipboard, but it doesn't send the whole string at once. It is sent in batches of 16 bytes with a 125ms delay between batches. These values can be tweaked with hidden settings. For example:

    defaults write com.googlecode.iterm2 SlowPasteBytesPerCall -int 16
    defaults write com.googlecode.iterm2 SlowPasteDelayBetweenCalls -float 0.125

#### Edit > Open Paste History...
"Open Paste History" opens a window showing up to the last 20 values that were copied or pasted in iTerm2. You can search its contents by typing a (non-necessarily-consecutive) subsequence of characters that appear in the value. You can use arrow keys and enter to make a selection, or you can click on an item to choose it, and it will be pasted. If you enable the Save copy/pate history to disk preference then these values will persist across sessions of iTerm2.
#### Edit > Open Autocomplete...
Shows the autocomplete window, which offers to finish typing a word that you've begun. <a href="documentation-highlights.html">Learn more about autocomplete on highlights page</a>.
#### Edit > Set Mark
Records the current scroll position. Use Edit > Jump to Mark to restore the scroll position.
#### View > Show Tabs in Fullscreen
If enabled, tabs are shown in fullscreen windows.
#### View > Use Transparency
This toggles transparency. It only has an effect if you have configured your session to be transparent under Preferences > Profiles > Window > Transparency. When Full Screen mode is entered, transparency is turned off by default, but you can select this menu item to re-enable it.
#### View > Find Cursor
Reveals the current cursor position.
#### View > Maximize Active Pane
When there are split panes present, this toggles whether a given pane expands to fill the tab. When a maximized pane is present, the tab will be inscribed with a dotted outline.
#### View > Edit Current Session
This opens a window that lets you change the settings of the current session without affecting any other sessions. Once this has been done, changes to the profile will not affect this session.
#### View > Step Back/Forward in Time
Stepping through time allows you to see what was on the screen at a previous time. This is different than going back through the scrollback buffer, as interactive programs sometimes overwrite the screen contents without having them scroll back. Once in this mode, you can use the left and right arrow keys to step back and forward, respectively. The "esc" key exits this mode, as does clicking the close button in the bar that appears on the bottom. You can adjust the amount of memory dedicated to this feature in Preferences > Instant Replay uses xx MB per session. The more memory you assign, the further back in time you can step.
#### View > Tab Color
Allows you to select a tint color for the tab, to make it easier to distinguish.
#### Profiles > Open Profiles...
This opens the "Profiles Window" which allows you to create new windows, tabs, or panes from one or more profiles. You can perform a search by entering text in the search field. Profile names and tags are searched, and the listed profiles are filtered as you type. You can use the up and down arrow keys to make a selection. Pressing enter will open a new tab, while shift-enter will open a new window. You can make multiple selections by holding down shift or cmd and clicking on profiles. The "New Tabs in New Window" button is enabled only when more than one profile is selected: it will open a new window and create a new tab for each profile selected.
#### Toolbelt > Show Toolbelt
This toggles the visibility of the Toolbelt on the right side of all windows.
#### Toolbelt > Jobs
This toggles the visibility of the Jobs tool, which shows the running jobs in the current session, and allows you to send them signals.
#### Toolbelt > Notes
This toggles the visibility of the Notes tool, which provides a freeform scratchpad in the toolbelt.
#### Toolbelt > Paste History
This toggles the visibility of the Paste History tool, which shows recently pasted strings in the toolbelt.
#### Toolbelt > Profiles
This toggles the visibility of the Profiles tool, which lets you select profiles to open new windows, tabs, and split panes.
#### Window > Exposé All Tabs
All iTerm2 tabs will be shown tiled on the main screen. You can mouse over a tab to see it larger, and clicking on it will restore the windows and select that tab and bring its window to the front. You can search the contents of all tabs by typing in the search field that appears on the left. Making a selection from the results below it will highlight the tab that contains that text. This is useful when you have many tabs open and can't find the one you're looking for.
#### Window > Save/Restore Window Arrangement
The current state and positions of windows, tabs, and spit panes is recorded and saved to disk with Save Window Arrangement. Restore Window Arrangement opens a new collection of windows having the saved state. You can automatically restore the arrangement in Preferences > General > Open saved window arrangement.
