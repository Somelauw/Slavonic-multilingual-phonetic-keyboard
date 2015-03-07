# Slavonic-multilingual-phonetic-keyboard
Phonetic keyboard layout for Russian and other Slavic languages.
This is a Linux version of the keyboard layout for Windows found [here](http://www.tyflonet.com/siciliano/kbdrutrl.zip).
It tries to be phonetic for qwerty users while supporting the most common Slavic languages with Cyrillic alphabets.
I created it using [Keyboard layout editor](https://github.com/simos/keyboardlayouteditor).

## Installation instructions:

1. Add layout.xml to the ru node in /usr/share/X11/xkb/rules/base.xml
2. Add layout.xml to the ru node in /usr/share/X11/xkb/rules/fdev.xml
3. Append layout.part to /usr/share/X11/xkb/symbols/ru

## Usage instructions
To use this layout either use setkdbmap (sets your keyboard layout for the current X session) or localetc (persistent).

For example to use Caps Lock as a toggle key between US and this layout use one of these commands:

    setxkbmap -model pc105 -layout us,ru -variant ,multilingual -option grp:caps_toggle

    localectl set-x11-keymap us,ru pc105 ,multilingual grp:caps_toggle

For more information about setting up your keyboard layout, consult [ArchWiki: Keyboard configuration in Xorg](https://wiki.archlinux.org/index.php/Keyboard_configuration_in_Xorg).

## Screenshot
![Screenshot](https://github.com/Somelauw/Slavonic-multilingual-phonetic-keyboard/blob/master/screenshot.png)

[Screenshot of the original](http://kbd-intl.narod.ru/images/ru-trl.png)

## Similar projects
A different project also supporting most Slavic languages based on the Russian Windows keyboard layout:
http://chuvash.eu/2015/01/03/creating-a-russian-extended-keyboard-layout/

Many keyboard layouts for different languages for windows can be found here (in fact this is where I found the original version of this layout) http://kbd-intl.narod.ru/english/layouts
