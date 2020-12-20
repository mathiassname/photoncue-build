# PhotonCUE

![Maintained][maintained-badge]
[![License](http://img.shields.io/badge/Licence-MIT-brightgreen.svg)](LICENSE.md)

[![Watch on GitHub][github-watch-badge]][github-watch]
[![Star on GitHub][github-star-badge]][github-star]
[![Tweet][twitter-badge]][twitter]

Kopiert [Mixed In Key](https://mixedinkey.com/) Cuepoints nach [Rekordbox](https://rekordbox.com/).

### Warum PhotonCUE?

PhotonCUE ist aus dem Problem heraus entstanden, dass keine freie und einfach zu nutzende Software existiert, welche die durch [Mixed In Key](https://mixedinkey.com/) erzeugten Cuepoints nach [Rekordbox](https://rekordbox.com/) importiert.

### Wie funktioniert PhotonCUE?

PhotonCUE nutzt den Export "Sammlung in XML-Format exportieren" von *Rekordbox* und gleicht die daraus resultierende XML-Datei mit der Datenbank von *Mixed in Key* ab.

#### Schritt für Schritt Anleitung

1. Tracks in *Mixed In Key* scannen und in *Rekordbox* importieren

    Scanne alle Tracks in *Mixed in Key* und importiere die Tracks danach in *Rekordbox*.
    
    ![Schritt 1](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_1.png)

1. Sammlung in XML-Format exportieren

    Öffne *Rekordbox* und navigiere zu dem Menüpunkt "Datei" und klicke danach auf "Sammlung in XML-Format exportieren". Über den sich öffnenden Dialog wird deine Sammlung als XML-Datei exportiert.

    ![Schritt 2](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_2.png)

1. Einstellungen von *Rekordbox* anpassen

    Öffne die "Voreinstellungen", diese findest du unter dem Menüpunkt "rekordbox". Navigiere in dem sich öffnenden Menü zu "Erweitert" und dem Tab "Datenbank" und passe den Pfad unter "Importierte Bibliothek" so an, dass dieser auf deine XML-Datei zeigt.

    ![Schritt 3](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_3.png)

1. PhotonCUE starten

    Starte nun *PhotonCUE* und wähle über "Rekordbox XML-Sammlung auswählen" den Pfad deiner XML-Datei aus. Wenn der Slider "Memory-CUE-Points überschreiben (Hotcues bleiben bestehen)" aktiviert ist, dann werden alle Memory-Cuepoints in der ausgewählten XML-Datei überschrieben. Hot Cues bleiben erhalten.

    ![Schritt 4](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_4.png)

1. CUE-Points kopieren

   Dazu einfach auf den Button "CUE-Points übertragen" klicken.

    ![Schritt 5.1](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_5_1.png)

   Es erscheint ein Ladespinner und wenn der Prozess beendet ist, erscheint in einem grauen Kasten eine Erfolgsmeldung.

    ![Schritt 5.2](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_5_2.png)

   Außerdem wurde ein Backup der originalen XML-Datei erzeugt.

    ![Schritt 5.3](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_5_3.png)

1. Importieren der Cuepoints

   Um die Cuepoints nach *Rekordbox* zu importieren muss in der Seitenleiste der Navigationspunkt "rekordbox xml" gewählt werden. Über "Alle Tracks" sollten nun alle Songtitel auffindbar sein mit einem Rechtsklick auf den gewünschten Songtitel und mit Klick auf "In Sammlung importieren" importierst du alle Informationen aus deiner XML-Datei neu in *Rekordbox*.

    ![Schritt 6.1](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_6_1.png)

   Wenn der Titel bereits in *Rekordbox* vorhanden ist, erscheint der folgende Dialog. Dieser muss mit "Ja" bestätigt werden.

    ![Schritt 6.2](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_6_2.png)
   
   *Wichtig*: Durch "In Sammlung importieren" werden deine bestehenden Daten für den jeweiligen Titel modifiziert bzw. überschrieben. Dieser Vorgang erfolgt auf eigene Gefahr.

1. Fertig

   Nun sollte wie im folgenden Screenshot zu sehen, die Memory-Cuepoints in *Rekordbox* enthalten sein.

    ![Schritt 7](https://github.com/mathiassname/photoncue-build/raw/main/documentation/img/step_7.png)

#### Hinweis

PhotonCUE generiert keine Hot Cues, sondern erzeugt nur Memory-Cuepoints. Dies hat den Grund, dass Hot Cues individuell selbst vergeben und nie automatisch durch ein Programm generiert werden sollten. 

### Systemanforderungen

Unter folgenden Anforderungen wurde PhotonCUE getestet:

* MacOS Catalina >= 10.15.0
* Rekordbox >= 5.8.0 oder >= 6.3.0
* Mixed In Key >= 8.5

### Bekannte Probleme

* Grid verschoben: In einigen Fällen sind die Cuepoints auf dem Grid, um eine viertel oder halbe Note verschoben

### Roadmap

Für die Weiterentwicklung von PhotonCUE sind bereits folgende Punkte auf der ToDo-Liste:

* Implementierung der Englischen Übersetzung von Texten
* Fehlerbehebung von bekannten Problemen
* Portierung auf Windows 10

### Wie kann ich helfen?

Es gibt viele Wege, wie du ein Projekt unterstützen kannst. Auf folgende Weise kannst du PhotonCUE unterstützen:

* Bugs melden: https://github.com/mathiassname/photoncue-build/issues/
* Teile PhotonCUE mit Freunden und Bekannten
* Buy me a coffee ☕️: https://www.paypal.com/donate/?hosted_button_id=G5QWZVJSCTRKA

[github-watch-badge]: https://img.shields.io/github/watchers/mathiassname/photoncue-build.svg?style=social
[github-watch]: https://github.com/mathiassname/photoncue-build/watchers
[github-star-badge]: https://img.shields.io/github/stars/mathiassname/photoncue-build.svg?style=social
[github-star]: https://github.com/mathiassname/photoncue-build/stargazers
[twitter]: https://twitter.com/intent/tweet?text=Check%20out%20PhotonCUE!%20https://github.com/mathiassname/photoncue-build%20%F0%9F%91%8D
[twitter-badge]: https://img.shields.io/twitter/url/https/github.com/mathiassname/photoncue-build.svg?style=social
[maintained-badge]: https://img.shields.io/badge/maintained-yes-brightgreen
