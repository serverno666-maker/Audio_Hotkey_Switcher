# Audio Hotkey Switcher Portable

Ein Windows-Tool zum Umschalten des Standard-Wiedergabegeräts per Hotkey. Die Version 1.1.3 läuft im Infobereich und kann optional mit Windows starten.

## Download

- [Programm für Windows (.exe)](https://github.com/serverno666-maker/Audio_Hotkey_Switcher/releases/latest/download/AudioHotkeySwitcherPortable.exe)
- [Vollständiger Quellcode mit Build-Dateien (.zip)](https://github.com/serverno666-maker/Audio_Hotkey_Switcher/releases/latest/download/AudioHotkeySwitcherPortable-source.zip)

## Verwendung

1. EXE starten und unter **Chose Speaker** und **Chose Headset** zwei aktive Wiedergabegeräte auswählen.
2. Unter **Set Hotkey** eine einzelne Taste festlegen. Die Vorgabe ist **F21**.
3. **Save & Exit** speichert die Auswahl und versteckt das Fenster im Infobereich. Das X versteckt das Fenster ebenfalls.
4. Über das Tray-Menü **Open** lässt sich das Fenster wieder öffnen; **Exit** beendet das Programm.

**Start with Windows** richtet beim Speichern den Autostart für den aktuellen Windows-Benutzer ein. Beim Windows-Start bleibt das Einstellungsfenster verborgen. Ein erneuter normaler Start öffnet das Fenster der laufenden Instanz.

## Aus dem Quellcode bauen

Benötigt wird Windows mit **.NET Framework 4.8**. Das Quellpaket enthält C#-Quelldateien, Symbole, den eingebetteten Audiohelfer und die Build-Skripte.

1. Quellpaket herunterladen und entpacken.
2. In Windows PowerShell im entpackten Ordner `./build.ps1` ausführen.
3. Die erstellte Datei liegt unter `bin/AudioHotkeySwitcherPortable.exe`.

`build.ps1` verwendet den mit .NET Framework verfügbaren C#-Compiler unter `%WINDIR%\Microsoft.NET\Framework\v4.0.30319\csc.exe`. Für die Symbole kann `generate_icons.ps1` die mehrstufigen Icons aus den enthaltenen Ausgangsdateien erneut erzeugen.

Die Quellversion enthält den aus dem bereitgestellten Programm stammenden Audiohelfer `SoundVolumeView.exe` und zwei ursprüngliche 16-Pixel-Symbole. Die gerätespezifischen Startwerte können nach dem ersten Start im Programm geändert werden.
