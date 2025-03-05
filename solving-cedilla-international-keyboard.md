First: **Make sure your keyboard is in the us-intl or us-altgr-intl layout** --> [[international-keyboard-br]]
## Edit the following files (if they exist):
```
sudo vim /usr/lib/gtk-3.0/3.0.0/immodules.cache
sudo vim /usr/lib/gtk-2.0/2.10.0/immodules.cache
```

- Alter the lines:
	"cedilla" "Cedilla" "gtk30" "/usr/share/locale" "az:ca:co:fr:gv:oc:pt:sq:tr:wa"

- to:
	"cedilla" "Cedilla" "gtk30" "/usr/share/locale" "az:ca:co:fr:gv:oc:pt:sq:tr:wa:en"
	
## Substitute "ć" for "ç" and "Ć" for "Ç" in /usr/share/X11/locale/en_US.UTF-8/Compose
```bash
sudo cp /usr/share/X11/locale/en_US.UTF-8/Compose /usr/share/X11/locale/en_US.UTF-8/Compose.bak

sed 's/ć/ç/g' < /usr/share/X11/locale/en_US.UTF-8/Compose | sed 's/Ć/Ç/g' > Compose

sudo mv Compose /usr/share/X11/locale/en_US.UTF-8/Compose
```

Them finally restart your computer.