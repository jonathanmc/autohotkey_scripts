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

; AppsKey remappings
AppsKey::AppsKey 	; makes AppsKey work, after remapping AppsKey below you need this.
			; can also use AppsKey::send {AppsKey}
; don't remap the AppsKey to Windows because it doesn't always work i.e. for Win+R it doesnt work
AppsKey & RShift::LWin	; this is another way to make a Win key
; RShift & AppsKey::LWin	; and this

; Left-handed Windows tabs
RAlt & ]::AltTab
RAlt & [::ShiftAltTab
RAlt & \::AltTab
; and, the same but with AppsKey
AppsKey & ]::AltTab					; tab window
AppsKey & [::ShiftAltTab				; tab window
AppsKey & \::SendInput, {LWinDown}{Tab}{LWinUp}	; win tab

AppsKey & End::SendInput, {CtrlDown}{w}{CtrlUp} ; soft close
AppsKey & Del::SendInput, {AltDown}{F4}{AltUp} 	; hard close
RAlt & Del::SendInput, {AltDown}{F4}{AltUp}	; hard close

AppsKey & Home::SendInput, {LWinDown}{Home}{LWinUp} ; special run window

AppsKey & Ins::SendInput, {CtrlDown}{Ins}{CtrlUp} ; paste?

; maps AppsKey to Windows key shortcuts
AppsKey & e::SendInput, {LWinDown}e{LWinUp} ; explorer
AppsKey & r::SendInput, {LWinDown}r{LWinUp} ; run
AppsKey & s::SendInput, {LWinDown}s{LWinUp} ; search
AppsKey & z::SendInput, {LWinDown}z{LWinUp} ; windows
AppsKey & h::SendInput, {LWinDown}h{LWinUp} ; voice typing
AppsKey & /::SendInput, {LWinDown}h{LWinUp} ; voice typing

AppsKey & v::SendInput, {LWinDown}v{LWinUp} ; clip
AppsKey & Up::SendInput, {LWinDown}{Up}{LWinUp}
AppsKey & Left::SendInput, {LWinDown}{Left}{LWinUp}
AppsKey & Right::SendInput, {LWinDown}{Right}{LWinUp}
AppsKey & Down::SendInput, {LWinDown}{Down}{LWinUp}
; WinMinimize, A
AppsKey & 1::SendInput, {LWinDown}1{LWinUp}
AppsKey & Numpad1::SendInput, {LWinDown}1{LWinUp}
AppsKey & 2::SendInput, {LWinDown}2{LWinUp}
AppsKey & Numpad2::SendInput, {LWinDown}2{LWinUp}
AppsKey & 3::SendInput, {LWinDown}3{LWinUp}
AppsKey & Numpad3::SendInput, {LWinDown}3{LWinUp}
AppsKey & 4::SendInput, {LWinDown}4{LWinUp}
AppsKey & Numpad4::SendInput, {LWinDown}4{LWinUp}
AppsKey & 5::SendInput, {LWinDown}5{LWinUp}
AppsKey & Numpad5::SendInput, {LWinDown}5{LWinUp}
AppsKey & 6::SendInput, {LWinDown}6{LWinUp}
AppsKey & Numpad6::SendInput, {LWinDown}6{LWinUp}
AppsKey & 7::SendInput, {LWinDown}7{LWinUp}
AppsKey & Numpad7::SendInput, {LWinDown}7{LWinUp}
AppsKey & 8::SendInput, {LWinDown}8{LWinUp}
AppsKey & Numpad8::SendInput, {LWinDown}8{LWinUp}

; CTRL+space = always on top
; ^+SPACE::  Winset, Alwaysontop, , A

