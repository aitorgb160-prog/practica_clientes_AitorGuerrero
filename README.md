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
![oracle](img/oracle.png)  
Creamos una conexión a Oracle con el usuario orauser, puerto 1521 y nombre de servicio FREEPDB1.  
![conexion](img/conexion.png)  
### 2. VS Code y extensión SQL Developer
El siguiente paso será descargar el paquete .deb actual de VS Code, e instalar una extension para oracle:    
![code](img/code.png)  
![ext](img/ext.png)  
![cone2](img/cone2.png)  
Comprobamos el funcionamiento:  
![sentencia](img/sentencia.png)  
### 3. SQL Plus
Descargaremos los ZIP Basic y sqlplus de la version 23.26.4.0.0 y hacemos conexión  
![plus](img/plus.png)  
### 4. SQLcl 
Instalamos java  
![java](img/java.png)  
Y nos descargamos el ZIP de SQLcl  
![sqlcl](img/sqlcl.png)  
Iniciamos una nueva terminal e iniciamos una conexión  
![term](img/term.png)  
### 5. PostgreSQL
Instalamos PostgreSQL  
![postgre](img/postgre.png)  
He tenido que editar el fichero de configuración de PostgreSQL para que la línea comentada de que escuche a todos esté operativa (descomentada) y el fichero para el usuario pguser para autorizarle acceso, los ficheros son estos: **/etc/postgresql/16/main/pg_hba.conf** y **/etc/postgresql/16/main/postgresql.conf**  
![todas](img/todas.png)  
![pguser](img/pguser.png)  
Una vez editados los ficheros de configuración, reiniciamos el servicio.  
![reinicio](img/reinicio.png)  
Y hacemos la conexión  
![cone](img/cone_post.png)  
### 6. Cliente gráfico pgAdmin 4
(no hecho)
### 7. Maria DB
Instalamos y hacemos una conexión  
![maria](img/maria1.png)  
Tenemos que editar la misma configuración que en PostgreSQL, que deje la conexión en todas las redes y permitir la autorización al usuario  
![maria](img/maria2.png)  
![maria](img/maria3.png)  
### 8. Clientes multi-SGBD
#### 8.1 DBeaver
Descargamos el paquete DEB actual  
![insta](img/insta.png)  
iniciamos tres conexiones  
![oracle](img/cone_oracle.png)  
![post](img/cone_postgre.png)  
![maria](img/cone_maria.png)  
He probado una consulta a cada una y funcionan correctamente.  
#### 8.2 Adminer
Instalamos Adminer  
![adminer](img/adminer.png)  
![adminer](img/adminer.png)  
He instalado las extensiones y comprobaremos la conexión  
![adminer](img/adminer_3.png)  
![adminer](img/adminer_4.png)
