字母键及数字键
```
    keycode 38 (keysym 0x61, a)
    keycode 56 (keysym 0x62, b)
    keycode 54 (keysym 0x63, c)
    keycode 40 (keysym 0x64, d)
    keycode 26 (keysym 0x65, e)
    keycode 41 (keysym 0x66, f)
    keycode 42 (keysym 0x67, g)
    keycode 43 (keysym 0x68, h)
    keycode 31 (keysym 0x69, i)
    keycode 44 (keysym 0x6a, j)
    keycode 45 (keysym 0x6b, k)
    keycode 46 (keysym 0x6c, l)
    keycode 58 (keysym 0x6d, m)
    keycode 57 (keysym 0x6e, n)
    keycode 32 (keysym 0x6f, o)
    keycode 33 (keysym 0x70, p)
    keycode 24 (keysym 0x71, q)
    keycode 27 (keysym 0x72, r)
    keycode 39 (keysym 0x73, s)
    keycode 28 (keysym 0x74, t)
    keycode 30 (keysym 0x75, u)
    keycode 55 (keysym 0x76, v)
    keycode 25 (keysym 0x77, w)
    keycode 53 (keysym 0x78, x)
    keycode 29 (keysym 0x79, y)
    keycode 52 (keysym 0x7a, z)
    keycode 19 (keysym 0x30, 0)
    keycode 10 (keysym 0x31, 1)
    keycode 11 (keysym 0x32, 2)
    keycode 12 (keysym 0x33, 3)
    keycode 13 (keysym 0x34, 4)
    keycode 14 (keysym 0x35, 5)
    keycode 15 (keysym 0x36, 6)
    keycode 16 (keysym 0x37, 7)
    keycode 17 (keysym 0x38, 8)
    keycode 18 (keysym 0x39, 9)
```
功能键
```
    keycode 67 (keysym 0xffbe, F1)
    keycode 68 (keysym 0xffbf, F2)
    keycode 69 (keysym 0xffc0, F3)
    keycode 70 (keysym 0xffc1, F4)
    keycode 71 (keysym 0xffc2, F5)
    keycode 72 (keysym 0xffc3, F6)
    keycode 73 (keysym 0xffc4, F7)
    keycode 74 (keysym 0xffc5, F8)
    keycode 75 (keysym 0xffc6, F9)
    keycode 76 (keysym 0xffc7, F10)
    keycode 95 (keysym 0xffc8, F11)
    keycode 96 (keysym 0xffc9, F12)
```
控制键
```
    keycode 50 (keysym 0xffe1, Shift_L)
    keycode 62 (keysym 0xffe2, Shift_R)
    keycode 37 (keysym 0xffe3, Control_L)
    keycode 105 (keysym 0xffe4, Control_R)
    keycode 64 (keysym 0xffe9, Alt_L)
    keycode 108 (keysym 0xffea, Alt_R)
    keycode 9 (keysym 0xff1b, Escape)
    keycode 22 (keysym 0xff08, BackSpace)
    keycode 36 (keysym 0xff0d, Return)
    keycode 118 (keysym 0xff63, Insert)
    keycode 119 (keysym 0xffff, Delete)
    keycode 112 (keysym 0xff55, PgUp)
    keycode 117 (keysym 0xff56, PgDn)
    keycode 110 (keysym 0xff50, Home)
    keycode 115 (keysym 0xff57, End)
    keycode 111 (keysym 0xff52, Up)
    keycode 116 (keysym 0xff54, Down)
    keycode 113 (keysym 0xff51, Left)
    keycode 114 (keysym 0xff53, Right)
    keycode 107 (keysym 0xff61, Print)
```
符号键
```
    keycode 20 (keysym 0x2d, minus)
    keycode 21 (keysym 0x3d, equal)
    keycode 34 (keysym 0x5b, bracketleft)
    keycode 35 (keysym 0x5d, bracketright)
    keycode 51 (keysym 0x5c, backslash)
    keycode 47 (keysym 0x3b, semicolon)
    keycode 48 (keysym 0x27, apostrophe)
    keycode 59 (keysym 0x2c, comma)
    keycode 60 (keysym 0x2e, period)
    keycode 61 (keysym 0x2f, slash)
    keycode 49 (keysym 0x60, grave)
```



组合键输入： 左shift1,2,3,q,w,e 与右shift1,2,3,q,w,e
```
    keycode 10 (keysym 0x21, exclam)
    keycode 11 (keysym 0x40, at)
    keycode 12 (keysym 0x23, numbersign)
    keycode 24 (keysym 0x51, Q)
    keycode 25 (keysym 0x57, W)
    keycode 26 (keysym 0x45, E)
    keycode 10 (keysym 0x21, exclam)
    keycode 11 (keysym 0x40, at)
    keycode 12 (keysym 0x23, numbersign)
    keycode 24 (keysym 0x51, Q)
    keycode 25 (keysym 0x57, W)
    keycode 26 (keysym 0x45, E)
```

我们看到，左shift+1, 右shift+1, 1的keycode 都是10，
但是，单按键10映射到0x31, 而shift键按下时映射到0x21
同样的keycode 24, 不按shift 映射到q, 按shift映射到Q

a.组合键盘keycode, 研究发现，ctrl+字母数字键，alt+字母数字键其keycode,及keysym与不按ctrl,alt一致
```

keycode 10 (keysym 0x31, 1)
keycode 11 (keysym 0x32, 2)
keycode 12 (keysym 0x33, 3)
keycode 24 (keysym 0x71, q)
keycode 25 (keysym 0x77, w)

keycode 26 (keysym 0x65, e)
```

可见keycode 是不变的，叫键盘扫描码， 根据不同状态映射成不同符号
b.键盘符号对应的英文名称,
state 含义还不是很清楚，当然是与状态有关，待叙吧。
```

state 0x11, keycode 49 (keysym 0x7e, asciitilde)
state 0x11, keycode 10 (keysym 0x21, exclam)
state 0x11, keycode 11 (keysym 0x40, at)
state 0x11, keycode 12 (keysym 0x23, numbersign)
state 0x11, keycode 13 (keysym 0x24, dollar)
state 0x11, keycode 14 (keysym 0x25, percent)
state 0x11, keycode 15 (keysym 0x5e, asciicircum)
state 0x11, keycode 16 (keysym 0x26, ampersand)
state 0x11, keycode 17 (keysym 0x2a, asterisk)
state 0x11, keycode 18 (keysym 0x28, parenleft)
state 0x11, keycode 19 (keysym 0x29, parenright)
state 0x11, keycode 20 (keysym 0x5f, underscore)
state 0x11, keycode 21 (keysym 0x2b, plus)
state 0x11, keycode 34 (keysym 0x7b, braceleft)
state 0x11, keycode 35 (keysym 0x7d, braceright)
state 0x11, keycode 51 (keysym 0x7c, bar)
state 0x11, keycode 47 (keysym 0x3a, colon)
state 0x11, keycode 48 (keysym 0x22, quotedbl)
state 0x11, keycode 59 (keysym 0x3c, less)
state 0x11, keycode 60 (keysym 0x3e, greater)
state 0x11, keycode 61 (keysym 0x3f, question)
state 0x11, keycode 62 (keysym 0xffe2, Shift_R)
state 0x10, keycode 23 (keysym 0xff09, Tab)
state 0x10, keycode 66 (keysym 0xffe5, Caps_Lock)
state 0x12, keycode 77 (keysym 0xff7f, Num_Lock)
state 0x2, keycode 37 (keysym 0xffe3, Control_L)
state 0x6, keycode 54 (keysym 0x43, C)
```
