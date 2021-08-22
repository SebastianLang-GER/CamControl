# CamControl
CamControl ist ein Hardware-Plugin, basierend auf einem ESP8266, zur Steuerung von beweglichen Überwachungskameras, die über EIA-485 und das Pelco "D"-Protokoll angesteuert werden.

## Funktionen
Das Gerät verfügt über einen automatischen und manuellen Steuerungsmodus mit Presets.
Weiterhin kann eine externe (priorisierte) Steuereinheit angeschlossen werden.
Eine Interaktion mit dem Gerät ist über eine REST-API und MQTT möglich.

## Bedienung
Die Überwachung, Steuerung und Konfiguration erfolgt über eine Progressive Web App im Webbrowser eines beliebigen Endgeräts.
Dazu müssen sich beide Geräte im selben Netzwerk befinden.
Für die Ersteinrichtung der WLAN-Zugangsdaten wird eine direkte WLAN-Verbindung über den Wireless Access Point (AP) des Hardware-Plugins mit einem Endgerät hergestellt.
Das Webinterface ist über die mDNS-URL "http://camcontrol.local" (Standardeinstellung) oder die zugewiesene IP-Adresse ("http://192.168.0.1" bei Verbindung über den AP) erreichbar.
Zur Verwendung von mDNS muss Bonjour für Windows oder Avahi für Linux installiert sein.
Android unterstützen mDNS derzeit leider nicht.
