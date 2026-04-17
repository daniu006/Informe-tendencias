# INDORME 1
## 1. Comandos Linux
En esta paractica usamos los comandos basicos de linux tanto para crear carpetas o archivos y eliminarlos o moverlos
## 2. Tiempo de duración
30 minutos
## 3. Fundamentos:

Uno de los conceptos más importantes es la gestión de archivos. En Linux, todo se maneja como archivos, por lo que aprender a manipularlos es fundamental. Comandos como `cp` permiten copiar archivos de un lugar a otro, mientras que `mv` se utiliza tanto para mover como para renombrar archivos. Por otro lado, `rm` elimina archivos y `rmdir` elimina directorios vacíos.

Además, se trabajó con redirecciones. El operador `>` permite sobrescribir el contenido de un archivo, mientras que `>>` agrega información sin borrar lo anterior.

También se utilizó el comando `cat`, que permite visualizar el contenido de archivos o redirigirlo hacia otros. Estas herramientas son esenciales para cualquier persona que quiera usar entornos Linux, ya que permite manejar información de manera rápida y eficiente.

## 4. Conocimientos previos.
   
Para realizar esta práctica, el estudiante necesita tener claros los siguientes temas:
- Comandos básicos de Linux
- Manejo de terminal
- Uso básico de un sistema operativo
- Navegación en directorios

## 5. Objetivos a alcanzar
   
- Implementar contenedores con nginx…..
- Manipular archivos de configuración…..
  
## 6. Equipo necesario

- Computador con sistema operativo Windows  
- WSL (Windows Subsystem for Linux) para ejecutar Linux  
- Terminal de comandos (bash)  
- Uso de redirecciones (`>`, `>>`) para manipulación de archivos  

---

## 7. Material de apoyo

- Documentación básica de comandos Linux  
- Guías proporcionadas por el docente  
- Recursos en línea sobre terminal Linux  

---

## 8. Procedimiento
 
**Paso 1:** Crear el directorio principal `proyecto_comandos`
 
```bash
mkdir proyecto_comandos
cd proyecto_comandos/
```
 
---
 
**Paso 2:** Crear subdirectorios: `documentos`, `imagenes`, `scripts`
 
```bash
mkdir documentos
mkdir imagenes
mkdir scripts
```
 
---
 
**Paso 3:** Crear el archivo `notas.txt` dentro de `documentos`
 
```bash
cd documentos/
touch notas.txt
```
 
---
 
**Paso 4:** Agregar contenido al archivo usando `echo` y `>>`
 
```bash
echo "Hola" >> notas.txt
echo "mundo" >> notas.txt
echo "soy" >> notas.txt
echo "danny" >> notas.txt
```
 
---
 
**Paso 5:** Copiar correctamente el archivo hacia la carpeta `scripts`
 
```bash
cd documentos/
cp notas.txt ../scripts/
cd ..
```
 
---
 
**Paso 6:** Renombrar el archivo a `backup_notas.txt` usando `mv`
 
```bash
cd scripts/
ls
mv notas.txt backup_notas.txt
ls
```
 
---
 
**Paso 7:** Copiar el archivo hacia la carpeta `imagenes`
 
```bash
cp backup_notas.txt ../imagenes/
cd ..
```
 
---
 
**Paso 8:** Eliminar el archivo en `imagenes` con `rm` y luego eliminar la carpeta con `rmdir`
 
```bash
cd imagenes/
ls
rm backup_notas.txt
cd ..
rmdir imagenes/
ls
```
 
---
 
**Paso 9:** Crear el archivo `resumen.txt` y copiar contenido con `cat` usando `>`
 
```bash
cd documentos/
touch resumen.txt
cat notas.txt > resumen.txt
```
 
---
 
**Paso 10:** Agregar una línea adicional usando `>>`
 
```bash
echo "esta es una linea adicional" >> resumen.txt
cd ..
```
 
---
 
**Paso 11:** Guardar el historial de comandos usando tubería (`history | tee archivo.txt`)
 
```bash
history | tee tarea-s1-Daniela_Abad.txt
```

---

## 9. Resultados esperados

Se logró crear y organizar correctamente una estructura de directorios y archivos utilizando comandos de Linux dentro de WSL. Se aplicaron operaciones como copiar, mover, renombrar y eliminar archivos.

Además, se comprendió el uso de redirecciones (`>` y `>>`) para manipular contenido dentro de archivos. Durante la práctica se presentaron errores comunes, especialmente en el manejo de rutas, los cuales fueron corregidos mediante el análisis y uso adecuado de comandos como `ls` y `cd`.

Finalmente, se generó un archivo con el historial de comandos ejecutados, evidenciando el proceso completo de la práctica.

---
## 10. Bibliografía
- Daniela, A. (2026). Comnados Linux.
