# Instalación de clientes para tres SGBD
### 1. Oracle Database 23ai Free
Instalamos un JDK compatible con la versión de SQL Developer descargada.
```
sudo apt install default-jdk unzip
java --version
```
![version](img/version.png)  
A continuación, descargaremos el ZIP de SQL Developer y lo descomprimremos en /opt  
![descom](img/descom.png)
Lo ejecutamos:  
![oracle](oracle.png)  
Creamos una conexión a Oracle con el usuario orauser, puerto 1521 y nombre de servicio FREEPDB1.  
![conexion](conexion.png)  
El siguiente paso será descargar el paquete .deb actual de VS Code:  
