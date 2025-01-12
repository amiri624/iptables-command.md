# iptables command


```bash
iptables --table TABLE -A/-C/-D... CHAIN- Regel --jump Ziel
```

```bash
iptables [-t Tabelle] --append [Kette] [Parameter]
```
```bash
iptables -t Filter --append INPUT -j DROP
```
```bash
iptables [-t Tabelle] --delete [Kette] [Regelnummer]
```
```bash
iptables -t filter --delete INPUT 2
```
```bash
iptables [-t Tabelle] --check [Kette] [Parameter]
```
```bash
iptables -t Filter --check INPUT -s 192.168.1.123 -j DROP
```
```bash
iptables [-t Tabelle] -A [Kette] -p {Protokollname} [Ziel]
```
```bash
iptables -t Filter -A INPUT -p udp -j DROP
```
```bash
iptables [-t Tabelle] -A [Kette] -s {Quelladresse} [Ziel]
```
```bash
iptables [-t Tabelle] -A [Kette] -s {Quelladresse} [Ziel]
```
```bash
iptables -t Filter -A INPUT -s 192.168.1.230 -j AKZEPTIEREN
```
```bash
iptables [-t Tabelle] -A [Kette] -d {Zieladresse} [Ziel]
```
```bash
iptables -t Filter -A Ausgabe -d 192.168.1.123 -j Drop
```
```bash
iptables [-t Tabelle] -A [Kette] -i {Schnittstelle} [Ziel]
```
```bash
iptables -t Filter -A INPUT -i wlan0 -j DROP
```
```bash
iptables [-t Tabelle] -A [Kette] [Parameter] -j {Ziel}
```
```bash
iptables -t Filter -A VORWÄRTS -j DROP
```
```bash
sudo iptables --flush
```
```bash
sudo iptables-speichern
```
```bash
sudo iptables-wiederherstellen
```
```bash
Sudo systemctl enable iptables
```
```bash
sudo iptables -L
```
