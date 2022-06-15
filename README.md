# Pepperl_Fuchs-LaserScannerR2000

Dieser Programmbaustein wurden entwickelt für Beckhoffs `TwinCAT 3`

## Beschreibung:
Dieser FB dient der Steuerung des 2D-LaserScanners OMDxxx–R2000 der Firma Pepperl + Fuchs in der Firmware Version 1.20.
Es werden lediglich Pakete des `Typs A` unterstützt!

```
Hier die Struktur des FB:

				 FB_LaserScannerR2000
				|		      |
				|		      |
				|		      V
				|		FB_httpClient
				|		      |
				|		      |
				V		      V	
			FB_UdpConnection	FB_TcpClient
				|		      |
				|		      |
				V		      V
			Beckhoff FBs		  Beckhoff FBs
```
