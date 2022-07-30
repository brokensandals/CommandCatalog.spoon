# CommandCatalog.spoon

A spoon (plugin) for [hammerspoon](https://www.hammerspoon.org) to help manage a command palette and associated hotkeys.
It keeps a list of commands which can be invoked via a fuzzy finder command palette.
If you also specify a hotkey when registering the command, the hotkey will be shown in the command palette too.

## Setup

Clone this repository inside of `~/.hammerspoon/Spoons`, then add `hs.loadSpoon("CommandCatalog")` to your `init.lua`.

## Usage

|Function name|Description|
|---|---|
|add(text, fn, [hotkeyMods, hotkeys])|Registers a command.|
|bindCommandHotkeys|Should be called once after all commands are registered.|
|chooseCommand|Shows a fuzzy finder with all registered commands.|
|sortCommands|Sorts the commands alphabetically - call this after all commands are registered, if you want.|

## License

This is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
