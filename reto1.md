# Lab 0 – Manejo básico de archivos en Linux

## 1. Crear el directorio solicitado

Se creó el directorio en la ruta especificada usando:

```bash
$ mkdir -p ~/operating-systems-20261/labs/reto0
```

La opción `-p` permite crear toda la estructura de carpetas si no existe.

## 2. Navegar al directorio creado

```bash
$ cd ~/operating-systems-20261/labs/reto0
```

## 3. Imprimir la ruta absoluta y enviarla a un archivo

```bash
$ pwd > path.txt
```

- `pwd` imprime la ruta absoluta.
- `>` redirige la salida al archivo `path.txt`.

## 4. Crear múltiples directorios con un solo comando

```bash
$ mkdir example music photos projects
```

Se crearon cuatro directorios simultáneamente.

## 5. Crear 100 archivos en cada directorio

```bash
$ touch example/file{1..100}
$ touch music/file{1..100}
$ touch photos/file{1..100}
$ touch projects/file{1..100}
```

- `{1..100}` es expansión de llaves (brace expansion).
- `touch` crea múltiples archivos en un solo comando.

## 6. Eliminar los primeros 10 y los últimos 20 archivos en cada directorio

```bash
$ rm example/file{1..10} example/file{81..100}
$ rm music/file{1..10} music/file{81..100}
$ rm photos/file{1..10} photos/file{81..100}
$ rm projects/file{1..10} projects/file{81..100}
```

Se eliminaron:
- Archivos del 1 al 10.
- Archivos del 81 al 100.

## 7. Mover los directorios a la carpeta projects

```bash
$ mv example music photos projects/
```

Se movieron los tres directorios dentro de projects.

## 8. Eliminar los archivos de projects con modo verboso y redirigir salida

```bash
$ rm -v projects/file* > ~/operating-systems-20261/labs/lab0.output.txt
```

- `-v` muestra los archivos eliminados.
- `file*` selecciona todos los archivos.
- `>` redirige la salida a `output.txt`.

## 9. Evidencia

Se adjuntan las siguientes imágenes:

1. Imagen con todos los comandos ejecutados.
2. Imagen mostrando los directorios creados.
3. Imagen mostrando los archivos dentro de las carpetas.
4. Imagen final mostrando la estructura después de mover y eliminar archivos.
