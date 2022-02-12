# autohotkey_scripts

Autohotkey scripts. Most for left-handed keyboard use. Edit into your autohotkey config file (AutoHotkey.ahk). Refresh. Comments inline.

```

; ^ = ctrl    ! = alt    + = shift



; Left-handed CUT COPY PASTE -> CTRL+number keys 1 2 3
^;::^x
^'::^c
^\::^v
;^Numpad1:: ^x
;^Numpad2:: ^c
;^Numpad3:: ^v
;^Ins::^v
;^Del::^x



; ALT-TAB -> makes right alt plus certain buttons mirror ALT+TAB
RAlt & \:: ShiftAltTab
RAlt & |:: AltTab
RAlt & [:: ShiftAltTab
RAlt & ]:: AltTab

AppsKey & ]::AltTab
AppsKey & [::ShiftAltTab
AppsKey & \::SendInput, {LWinDown}{Tab}{LWinUp}

AppsKey & e::SendInput, {LWinDown}e{LWinUp}
AppsKey & z::SendInput, {LWinDown}z{LWinUp}
AppsKey & v::SendInput, {LWinDown}v{LWinUp}
AppsKey & /::SendInput, {LWinDown}h{LWinUp} ;voice typing

; maps AppsKey to behave like Win for minimizing, maximizing and close
AppsKey & Up::SendInput, {LWinDown}{Up}{LWinUp}
AppsKey & Left::SendInput, {LWinDown}{Left}{LWinUp}
AppsKey & Right::SendInput, {LWinDown}{Right}{LWinUp}
AppsKey & Down::SendInput, {LWinDown}{Down}{LWinUp}

AppsKey & End::SendInput, {CtrlDown}{w}{CtrlUp}		; CTRL-W close
AppsKey & Del::SendInput, {AltDown}{F4}{AltUp}		; hard close



; CTRL+space = always on top
; ^+SPACE::  Winset, Alwaysontop, , A

