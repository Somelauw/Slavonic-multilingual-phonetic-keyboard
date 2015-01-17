# Slavonic-multilingual-phonetic-keyboard
Phonetic keyboard for Russian and other languages
Is a linux port from the windows keyboard layout found here: http://www.tyflonet.com/siciliano/kbdrutrl.zip

Add layout.xml add the ru node in /usr/share/X11/xkb/rules/base.xml
Add layout.xml add the ru node in /usr/share/X11/xkb/rules/fdev.xml
Add layout.part to /usr/share/X11/xkb/symbols/ru

To temporarily try it

    setxkbmap -model pc105 -layout us,ru -variant altgr-intl,multilingual -option grp:caps_lock

To set it as default

    localectl set-x11-keymap us,ru pc105 altgr-intl,multilingual grp:caps_lock

I created it using https://github.com/simos/keyboardlayouteditor
