# nautilus-pfad-kopieren
Eine kleine Nautilus-Erweiterung zum schnellen Kopieren von Datei-/Samba-Pfaden.

![Screenshot](https://github.com/pappmann/nautilus-pfad-kopieren/screenshots/Bildschirmfoto.png)

## Installation aus dem Quellcode
Um das Plugin erfolgreich zu installieren, brauchst du:
1. Python >= 3.2
2. GNOME >= 3.18 (getestet unter Debian 10-12, Ubuntu 16.04-22.04, Fedora 25-37, Arch Linux)
3. GObject Python-Bindings (Entwicklungsbibliotheken)
4. nautilus-python

### Installation der Abhängigkeiten
Kopiere einfach den für deine Distribution passenden Befehl und füge ihn ein:

| Distribution | Befehl|
|--------|--------|
| Fedora | ``` $ sudo dnf install nautilus-python python3-gobject ``` |
| Debian >= 12 | ``` $ sudo apt install python3-nautilus python3-gi ``` |
| Ubuntu | ``` $ sudo apt-get install python-nautilus python3-gi ``` |
| Arch Linux | ``` $ sudo pacman -S python-gobject python-nautilus ``` |

### Installation der Erweiterung
Klon das Repository:
```
git clone https://github.com/ronen25/nautilus-copypath
```

Kopiere die Datei(en) in den entsprechenden Ordner und erstelle ihn bei Bedarf:
```bash
$ mkdir ~/.local/share/nautilus-python
$ mkdir ~/.local/share/nautilus-python/extensions
$ cp nautilus-copypath.py ~/.local/share/nautilus-python/extensions/
```

Starte Nautilus neu, damit die Erweiterung verfügbar ist:
```bash
$ nautilus -q
```

Wenn das nicht klappt, versuch dich mal ab- und wieder anzumelden. 
