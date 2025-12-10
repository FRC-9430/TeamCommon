# Configuring Your Environment

It is important each environment's formatting settings remain the same for
the consistency of our codebase. It also ensures we can effortlessly follow our code style guide without much effort into thinking about where symbols go.

To configure your environment, please follow this guide to get on the same page as the rest of your team. Feel free to tweak some of the configurations as you like, but remember that your settings should ultimately format your code according to our repository code standards.

## Prerequisites

1. VSCode W/ WPILib must be installed "For All Users" during installation via ISO.
    An admin may need to assist with this installation.
2. Modify settings.json to ensure the paths to WPILib are correct. Use CTRL+H/Find and replace.
    You will receive errors notifying you that a path to your JVM is invalid.
3. Modify snippets in `snippets/` to match your name and username as
    prompted by the comments in the file.

## Configuration Process

1. Place completed `settings.json` and `snippets/` folder into `{PATH TO WPILIB}/vscode/VSCode-{PLATFORM}/data/user-data/User`
2. Open VSCode for WPILib and ensure you don't get errors on startup. See below for [Troubleshooting](#troubleshooting)
3. Open the VSCode Extensions view on the left sidebar (or CTRL+SHIFT+X). Pasting 5 extension IDs at a time in the search bar, install/update all extensions for your user profile. *Note: you will not be able to see all extensions if you paste them all at the same time*

At the end of this process, you should be able to see some new changes to various parts of the WPILib/VSCode UI.

## Summary of Configurations

1. Disabled automatic Microsoft Copilot chat agent and AI features
2. Quality of Life configs let you hit "Enter" without necessarily accepting IDE suggestions (Hit TAB instead)
3. Parameter values in functions should show up during development
4. The editor will automatically format code as you type or paste code
5. Whitespace characters (spaces and tabs) will be visible in all files
6. Tabs will be converted to 4 spaces, but will still be backspaced like tabs
7. Intuitive minimap settings to scroll easier through large files
8. Pre-Configured todo-tree settings which will allow us to summarize and count various tags (TODO/FIXME/REVIEW/NOTE/HELP/MERGE CONFLICT) in our codebase
9. Faint vertical markers ("rulers") to help visualize long lines of code relative to standard 80/120 characters

You are free to make additional tweaks to your environment to personalize it and make it your own. You are also welcome to update enable additional features you believe will assist you in your development. However, **all formatting options must remain consistent with our repository conventions.** Code style will be subject to peer review, and differences in conventions will create issues in collaboration later.

## Troubleshooting

**If you're getting JVM startup errors**: Run a quick code build if you want a sanity check, and verify it uses the JDK from your **WPILib Home Directory**. If you see something like "`C:\Program Files\Java\...`", you will need to double check your settings/configs.
