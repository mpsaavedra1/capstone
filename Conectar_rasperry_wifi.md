# CONECTAR RASPERRY PI 4 AL WIFI

1. Debemos editar el fichero /etc/wpa_supplicant/wpa_supplicant.conf
```
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
```
2. En el fichero se añade nuestra red wifi 

```
network={
        ssid="NOMBRE_RED"
        psk="CONTRASEÑA_RED"
        key_mgmt=WPA-PSK
}
```
*Para guardar cambios con CTRL+0, luego Enter y finalmente CTRL+X

3. Reiniciamos rasperry pi
sudo reboot

4. Comprobar conectado correctamente y obtener IP
ifconfig wlan0

# https://www.luisllamas.es/raspberry-pi-wifi/
