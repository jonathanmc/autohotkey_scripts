# autohotkey_scripts

Autohotkey scripts. Most for left-handed keyboard use. Put in your autohotkey config file. Refresh. Comments inline.

```
; ^ = ctrl    ! = alt    + = shift

; ALT-TAB -> makes right alt plus certain buttons mirror ALT+TAB
RAlt & \:: ShiftAltTab
RAlt & |:: AltTab
RAlt & [:: ShiftAltTab
RAlt & ]:: AltTab

; q::Tab

; Left-handed CUT COPY PASTE -> CTRL+number keys 1 2 3
;^Numpad1:: ^x
;^Numpad2:: ^c
;^Numpad3:: ^v
;^Ins::^v
;^Del::^x

; Left-handed CUT COPY PASTE -> CTRL+; +' and +\
^;::^x
^'::^c
^\::^v

; CTRL+space = always on top
; ^+SPACE::  Winset, Alwaysontop, , A

; makes CTRL + 0 = ALT + `
;^`::^Numpad0
; `::MsgBox, BackTick Pressed
```
