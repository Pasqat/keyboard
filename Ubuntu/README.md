You need to restart your computer.

Use
```
sudo cat better-prog-dvorak >> /usr/share/X11/xkb/symbols/us
```

Then update `sudo nvim /usr/share/X11/xkb/rules/evdev.xml` with the following, just
after "dvorak-classic"

```
        <variant>
          <configItem>
            <name>real-prog-dvorak</name>
            <description>English (Real programmer Dvorak)</description>
            <vendor>Pasquale Matarrele</vendor>
          </configItem>
        </variant>
```
