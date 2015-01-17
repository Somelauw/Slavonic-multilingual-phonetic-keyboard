# Slavonic-multilingual-phonetic-keyboard
Phonetic keyboard layout for Russian and other languages.
This is a linux port from the windows keyboard layout found here: http://www.tyflonet.com/siciliano/kbdrutrl.zip .
I created it using https://github.com/simos/keyboardlayouteditor .

Installation instructions:

1. Add layout.xml to the ru node in /usr/share/X11/xkb/rules/base.xml
2. Add layout.xml to the ru node in /usr/share/X11/xkb/rules/fdev.xml
3. Append layout.part to /usr/share/X11/xkb/symbols/ru

To use this layout either use setkdbmap (sets your keyboard layout for the current X session) or localetc (persistent).

For example to use Caps Lock as a toggle key between US and this layout use one of these command:

    setxkbmap -model pc105 -layout us,ru -variant ,multilingual -option grp:caps_lock

    localectl set-x11-keymap us,ru pc105 ,multilingual grp:caps_lock

For more information about setting up your keyboard layout, consult https://wiki.archlinux.org/index.php/Keyboard_configuration_in_Xorg

