# Export der Network Devices und deren IP-Adressen aus der ISE in je eine Datei.
## ansible.cfg
Diese Datei enthält die Konfiguration für die Ansible Umgebung
## Verzeichnis "inventory"
Hier befinden sich die exportierten "Network Device" aus der ISE.
### hosts_dev.ini
Diese Datei enthält den Inhalt des Export aus der ISE.
Der Name der Datei ist der Name des "Network Device" innerhalb der ISE.
Der Inhalt der Datei ist/sind die IP-Adressen, welche ind er "Network Device" konfiguriert wurden.
## Datei hosts
Diese Datei beinhaltet die Ansteuerung der ISE.
# Ausführen des Exports
```
ansible-playbook -i hosts network_device.yml 
```
