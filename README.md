# Audio Hotkey Switcher Portable

Windows-Tool zum Umschalten des Standard-Multimedia-Wiedergabegeräts per Hotkey. Version **1.1.4** benötigt **64-Bit-Windows** und **.NET Framework 4.8**.

## Download

- [Programm für Windows (ZIP)](https://github.com/serverno666-maker/Audio_Hotkey_Switcher/releases/latest/download/AudioHotkeySwitcherPortable-v1.1.4-windows-x64.zip)
- [Vollständiger Quellcode und Build-Dateien (ZIP)](https://github.com/serverno666-maker/Audio_Hotkey_Switcher/releases/latest/download/AudioHotkeySwitcherPortable-v1.1.4-source.zip)

Das Programm-ZIP vollständig entpacken und **AudioHotkeySwitcherPortable.exe** starten. Der Ordner **SoundVolumeView** muss neben der EXE bleiben. Eine einzeln herauskopierte EXE kann das Wiedergabegerät nicht wechseln.

## Verwendung

1. Unter **Chose Speaker** und **Chose Headset** zwei aktive Wiedergabegeräte auswählen.
2. Unter **Set Hotkey** eine einzelne Taste festlegen. Vorgabe: **F21**.
3. **Save & Exit** speichert die Auswahl und versteckt das Fenster im Infobereich. Das X versteckt das Fenster ebenfalls.
4. Im Tray-Menü öffnet **Open** das Fenster wieder; **Exit** beendet das Programm.

**Start with Windows** richtet beim Speichern den Autostart für den aktuellen Windows-Benutzer ein. Beim Windows-Start bleibt das Einstellungsfenster verborgen.

## Aus dem Quellcode bauen

Das Quellpaket enthält C#-Quelldateien, Symbole, Build-Skripte und das unveränderte offizielle 64-Bit-Distributionsarchiv von SoundVolumeView 2.53. Unter Windows mit .NET Framework 4.8 das Quellpaket entpacken und in Windows PowerShell **.\build.ps1** ausführen. Die Laufzeitdateien liegen danach zusammen unter **bin**. Das Skript prüft den SHA-256-Wert des NirSoft-Archivs, verwendet den .NET-Framework-C#-Compiler und entpackt alle Dateien des Helfers.

SoundVolumeView ist Freeware von [NirSoft](https://www.nirsoft.net/utils/sound_volume_view.html). Die mitgelieferte **SoundVolumeView/readme.txt** enthält dessen Lizenz: kostenlose Weitergabe außerhalb kommerzieller Produkte nur mit allen unveränderten Distributionsdateien. Das Programm-ZIP enthält die EXE, Hilfedatei und readme.txt des Helfers sowie das unveränderte Originalarchiv.

## Prüfsummen (SHA-256)

- Programm-ZIP: `7904F35E18E1697F55072BA663C85979C1452FA3E0BF279CB479E3EE617E669C`
- Quellpaket: `81332A12136257D15B7FC98D2854C58AEB9DA70C06FC76F9832B6841651202E4`
