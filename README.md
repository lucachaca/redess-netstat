# Escáner de Red - Java

## 📖 Descripción
Este programa permite escanear un rango de direcciones IP de tu red local, verificar si están activas, medir el tiempo de respuesta en milisegundos y obtener el nombre del host asociado.  

Los resultados se muestran en una **interfaz gráfica** y se pueden guardar en un archivo **CSV** para abrir en Excel.  

---

## 📋 Requisitos
- Tener instalado **Java JDK 8 o superior**.  
- Sistema operativo con soporte para:
  - `InetAddress.isReachable()`
  - `nslookup` (Windows, Linux o macOS).  

---

## ▶️ Cómo usar el programa

### 1. Ejecutar el programa
Abre una terminal o tu IDE favorito.  

Compila y ejecuta el proyecto:

```bash
javac red/*.java
java red.Main
Se abrirá una ventana con el menú principal donde podrás elegir:

Escáner de Red

Netstat Viewer

2. Ingresar el rango de IPs
En el campo “IP Inicio”, escribe la primera IP del rango que quieras escanear.
En el campo “IP Fin”, escribe la última IP del rango.

Ejemplo:

nginx
Copiar código
IP Inicio: 192.168.1.1
IP Fin:    192.168.1.10
3. Escanear
Presiona el botón “Escanear”.

La tabla se llenará con:

IP: dirección IP escaneada

Activo: SI/NO según si responde al ping

Tiempo (ms): tiempo de respuesta en milisegundos

Nombre Host: nombre del host (si está disponible)

4. Guardar resultados
Presiona el botón “Guardar” para generar un archivo resultado_ping.csv.

Este archivo se crea en la misma carpeta del programa y puede abrirse con Excel.

5. Limpiar la tabla
Presiona el botón “Limpiar” para borrar los resultados actuales y poder hacer un nuevo escaneo.

⚠️ Notas importantes
El tiempo de respuesta depende de la red y del sistema operativo, por lo que puede variar ligeramente.

La función de host requiere que nslookup esté disponible en tu sistema.

Para rangos grandes, el escaneo puede tardar algunos segundos por cada IP.

css
Copiar código
