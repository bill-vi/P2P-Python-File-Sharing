# P2P-Python-File-Sharing

Este proyecto es una aplicación web ligera desarrollada con **Python** y **Flask** que permite compartir archivos entre dispositivos conectados a la misma red local. El objetivo es que un usuario pueda subir archivos desde su PC o dispositivo móvil y que otros puedan descargarlos accediendo a una interfaz web. La aplicación implementa un servidor básico P2P, accesible desde cualquier dispositivo de la red, permitiendo compartir archivos fácilmente.

## Requerimientos

- **Python 3.x**

### Librerías y Dependencias
- **Flask**: Para crear el servidor web.
- **OS**: Para gestionar el sistema de archivos local.

## Ejecucición

### Clonar Repositorio

```bash
git clone https://github.com/usuario/server-p2p-python-flask.git
cd server-p2p-python-flask
```

### Crear Entorno Virtual
1. Abre una Terminal.
2. Ve al directorio de tu proyecto.
3. Crea el entorno virtual usando el siguiente comando

```bash
python3 -m venv nombre_del_entorno # Linux/Mac
python -m venv nombre_del_entorno # Windows
```
Reemplaza `nombre_del_entorno` por el nombre que quieras darle al entorno virtual.

```bash
source nombre_del_entorno/bin/activate  # Linux/Mac
nombre_del_entorno\Scripts\activate   # Windows
```

### Instalar Flask
```bash
pip install flask
```
### Ejecución en Windows
1. Abre una terminal y navega a la carpeta del proyecto.
2. Ejecuta el siguiente comando para iniciar el servidor:
```bash
python app.py
```
3. El servidor Flask se ejecutará por defecto en el puerto 5000. Si deseas cambiar el puerto:
```bash
python app.py 5001
```
4. Accede a la aplicación web desde tu navegador ingresando:
```bash
http://<dirección-de-ip_de_tu_pc>:5000
```

### Ejecución en Linux
1. Abre una terminal y navega a la carpeta del proyecto.
2. Si estás utilizando un firewall como ufw, permite el acceso al puerto 5000 (u otro puerto si lo especificaste):
```bash
sudo ufw allow 5000
```
3. Ejecuta el siguiente comando para iniciar el servidor:
```bash
python app.py
```
4. Accede a la aplicación web desde tu navegador ingresando:
```bash
http://<dirección-de-ip_de_tu_pc>:5000
```

### Ejecución en Mac
1. Abre una terminal y navega a la carpeta del proyecto.
2. Ejecuta el siguiente comando para iniciar el servidor:
```bash
python app.py
```
3. Accede a la aplicación web desde tu navegador ingresando:
```bash
http://<dirección-de-ip_de_tu_pc>:5000
```

### Acceder desde un Teléfono Inteligente
1. Asegúrate de que tanto el PC como el dispositivo móvil están conectados a la **misma red local**.
2. Abre el navegador web en tu teléfono móvil y accede a la IP local de la máquina donde está corriendo el servidor Flask. Usa la dirección IP de tu máquina seguida del puerto donde corre la aplicación, por ejemplo:
```bash
http://192.168.x.xxx:5000
```
Donde `192.168.x.xxx` es la IP local de tu PC. Puedes verificar la IP de tu máquina ejecutando `ipconfig` en Windows o `ifconfig` en Linux/Mac.

### Importante
- Asegúrate de que el puerto que estás utilizando esté **permitido por tu firewall**.
- Si ejecutas múltiples instancias del servidor en la misma máquina, asegúrate de **especificar puertos diferentes para cada una**.








