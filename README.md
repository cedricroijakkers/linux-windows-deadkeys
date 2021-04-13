# linux-windows-deadkeys

## Introduction

This `.XCompose` file allows you to use the "English (US, intl., with dead keys)" keyboard in Linux just like you would in Windows.

The behaviour of dead keys in Linux is slightly different than in Windows. If you are switching from Windows to Linux, and you are used to using your dead keys in a particular way, this can be quite annoying. Luckily, Linux allows you to customise pretty much anything, and dead key behaviour is one of those things.

## How to use it

All you need to do is download the file `XCompose` from this repository, and save it as `~/.XCompose` (i.e. in your home directory) and log out and back in from your desktop environment (i.e. Gnome).

Or, in one command:

```sh
curl https://raw.githubusercontent.com/cedricroijakkers/linux-windows-deadkeys/main/XCompose > ~/.XCompose
```

## Customisations

If you don't like how some dead keys are working now, you are of course free to modify them to your liking. Just open the file `~/.XCompose` in your favourite editor, and change anything you want. On each line, the file expects an entry like the following:

```
<first (dead) key> <second key> : "resulting characters"
```

So if you want the keystroke `'` + `c` to result in the character `ć`, look for the line:

```
<dead_acute> <c> : "ç"
```

And replace it with:

```
<dead_acute> <c> : "ć"
```

Or any other character of your liking. Save and close the file, and re-log in to your desktop environment.