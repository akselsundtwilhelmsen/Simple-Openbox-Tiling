# Super simple manual tiling for Openbox

![Demonstration](https://i.imgur.com/lohHHFN.gifv)

Just add the following in your <keyboard> section of your `/.config/openbox/rc.xml` and restart Openbox.

```
    <keybind key="W-S-h">
      <action name="MoveResizeTo">
        <x>0</x>
        <y>0</y>
        <width>1/2</width>
        <height>1/1</height>
      </action>
    </keybind>
    <keybind key="W-S-l">
      <action name="MoveResizeTo">
        <x>-0</x>
        <y>0</y>
        <width>1/2</width>
        <height>1/1</height>
      </action>
    </keybind>
    <keybind key="W-S-k">
      <action name="MoveResizeTo">
        <y>0</y>
        <width>1/2</width>
        <height>1/2</height>
      </action>
    </keybind>
    <keybind key="W-S-j">
      <action name="MoveResizeTo">
        <y>-0</y>
        <width>1/2</width>
        <height>1/2</height>
      </action>
    </keybind>
    <keybind key="W-S-h">
      <action>
        <x>0</x>
        <y>-0</y>
        <width>1/2</width>
        <height>1/2</height>
      </action>
    </keybind>
```

Super(win) + Shift + Vim keys `hjkl` are used to resize and move the windows.

*Note: Some terminals such as URxvt doesn't support per pixel resizing, but others such as Terminator and ST with (this)[https://st.suckless.org/patches/anysize/] patch supports it.*
