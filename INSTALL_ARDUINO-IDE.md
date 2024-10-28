
Descargar archivo `.zip` para Linux de ARDUINO IDE de la página ofcial https://www.arduino.cc/en/software 
### Descomprime el archivo
En este caso se ha descargado el archov `arduino-ide_2.3.3_Linux_64bit.zip` dirigirse al directorio del archivo y descomprimirlo en una carpeta específica y luego ingresa al directorio que se ha creado
```bash
unzip arduino-ide_2.3.3_Linux_64bit.zip
cd arduino-ide_2.3.3_Linux_64bit
```
luego entrar al directorio 
### Configuración de permisos

Cambia los permisos de `chrome-sandbox`para evitar problemas con la ejecución

```bash
sudo chown root chrome-sandbox
sudo chmod 4755 chrome-sandbox
```

### Creación de un enlace simbólico
Con esto se podrá invocar arduino-ide desde cuanquier ubicación
```bash
sudo ln -s /home/tarchies/software/arduino-ide_2.3.3_Linux_64bit/arduino-ide /usr/local/bin/arduino-ide
```

### Ejecución de arduino-ide
Ya puedes ejecutar arduino IDE desde cualquier directorio

```bash
arduino-ide &
```
  si tiene problemas con el uso de la GPU puedes evitar los problemas de compatibilidad gráfica con 

```bash
arduino-ide --disable-gpu &
```

