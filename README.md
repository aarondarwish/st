# st
A modified suckless terminal with a volcano theme.

To install, execute:
```bash
git clone https://github.com/aaron-darwish/st ~/.st
cd ~/.st
sudo make install
```
If you make a change and wish for it to take effect, simply run:
```bash
cd ~/.st
sudo make clean install
```

Run picom in the background to add a transparency effect:
```console
picom -cfF -o 0.38 -O 200 -I 200 -t 0 -l 0 -r 3 -D2 -m 0.88
```
Though `picom -c -b` should suffice as the former flag enables a shadows effect, and the latter autostarts picom as a background process.
Add it to your `.xinitrc` file in order for it to run on startup, assuming you are running the **X.Org Server**.
