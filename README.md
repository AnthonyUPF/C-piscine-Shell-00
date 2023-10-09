# C Piscine - Shell 00

Este documento corresponde al enunciado del módulo Shell 00 de la C Piscine de 42.

## Instrucciones

- Los ejercicios han sido ordenados con mucha precisión, del más sencillo al más complejo. En ningún caso se tendrá en cuenta un ejercicio complejo si no se ha conseguido realizar perfectamente un ejercicio más sencillo.
- Asegúrate de que tus directorios y archivos tienen los permisos adecuados.
- Debes respetar el procedimiento de entrega para todos tus ejercicios.
- Además de por tus compañeros, también serán corregidos por un programa que se llama la Moulinette.
- La Moulinette es muy estricta a la hora de evaluar. Está completamente automatizada. Es imposible discutir con ella sobre tu nota. Por lo tanto, se extremadamente riguroso para evitar cualquier sorpresa.
- Los ejercicios shell se deben ejecutar con /bin/sh.
- No puedes dejar en tu directorio ningún archivo que no se haya indicado de forma explícita en los enunciados de los ejercicios.
- Lee detenidamente los ejemplos. Podrían exigir cosas que no se especifican necesariamente en los enunciados. . .

## Ejercicio 00: Z

**Directorio de entrega**: `ex00/`

**Archivos a entregar**: `z`

**Funciones autorizadas**: Ninguna

### Instrucciones
Crea un archivo `z` que, cuando se ejecute un `cat` sobre él, muestre "Z" seguido de un salto de línea.

- Ejemplo:
  
  ```
  ?>cat z
  Z
  ?>
  ```

## Ejercicio 01: testShell00

**Directorio de entrega**: `ex01/`

**Archivos a entregar**: `testShell00.tar`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea el archivo `testShell00` en tu directorio de entrega.
- Encuentra la manera de que tu pantalla muestre lo siguiente (excepto por la línea de “total 1”):
  ```
  %> ls -l
  total XX
  -r--r-xr-x 1 XX XX 40 Jun 1 23:42 testShell00
  %>
  ```
- Una vez completados los pasos anteriores, ejecuta el siguiente comando para crear el archivo que debe ser entregado: tar -cf testShell00.tar testShell00.
- No te preocupes por lo que aparece en lugar de “XX”.
- Se acepta un año como respuesta en lugar de la hora.

## Ejercicio 02: Sí, quiero más...

**Directorio de entrega**: `ex02/`

**Archivos a entregar**: `exo2.tar`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea los siguientes archivos y directorios. Haz lo que sea necesario para que la ejecución de un `ls -l` en tu directorio muestre algo que se parezca a esto:

  ```
  %> ls -l
  total XX
  drwx--xr-x 2 XX XX XX Jun 1 20:47 test0
  -rwx--xr-- 1 XX XX 4 Jun 1 21:46 test1
  dr-x---r-- 2 XX XX XX Jun 1 22:45 test2
  -r-----r-- 2 XX XX 1 Jun 1 23:44 test3
  -rw-r----x 1 XX XX 2 Jun 1 23:43 test4
  -r-----r-- 2 XX XX 1 Jun 1 23:44 test5
  lrwxrwxrwx 1 XX XX 5 Jun 1 22:20 test6 -> test0
  %>
  ```
- Una vez resuelto el ejercicio, ejecuta el comando tar -cf exo2.tar * para crear el archivo que tendrás que entregar.
- No te preocupes por lo que aparece en lugar de “XX”.
- Se acepta un año como respuesta en lugar de la hora.

## Ejercicio 03: ¡Conéctame por SSH!

**Directorio de entrega**: `ex03/`

**Archivos a entregar**: `id_rsa_pub`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea tu propia clave SSH. Cuando lo tengas:
  - Añade tu clave pública a tu repositorio, en un archivo `id_rsa_pub`.
  - Actualiza tu clave ssh en la intranet. Esto te permitirá lanzar el repositorio a nuestro servidor git.
- El nombre del archivo no ha sido elegido de manera aleatoria.
- Asegúrate de entender la diferencia entre clave pública y clave privada.

## Ejercicio 04: midLS

**Directorio de entrega**: `ex04/`

**Archivos a entregar**: `midLS`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea en un archivo `midLS` que contenga el comando que hay que ejecutar para listar los archivos y los directorios del directorio actual, pero no los archivos ocultos, ni "." ni ".." (nada que empiece con un punto), separados por una coma y un espacio, ordenados por fecha de modificación y de tal modo que los directorios vayan seguidos por el carácter slash ("/").
- ¡No hay que hacer lo que no se ha pedido!

## Ejercicio 05: GiT commit

**Directorio de entrega**: `ex05/`

**Archivos a entregar**: `git_commit.sh`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea un script de shell que muestre en pantalla los id de los últimos 5 commits de tu repositorio git.
  
- Ejemplo:
  ```
  %> bash git_commit.sh | cat -e
  baa23b54f0adb7bf42623d6d0a6ed4587e11412a$
  2f52d74b1387fa80eea844969e8dc5483b531ac1$
  905f53d98656771334f53f59bb984fc29774701f$
  5ddc8474f4f15b3fcb72d08fcb333e19c3a27078$
  e94d0b448c03ec633f16d84d63beaef9ae7e7be8$
  %>
  ```
- Para probar tu script, utilizaremos nuestro propio entorno.

## Ejercicio 06: gitignore

**Directorio de entrega**: `ex06/`

**Archivos a entregar**: `git_ignore.sh`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea un script de shell que muestre por pantalla la lista de archivos existentes ignorados por tu repositorio git actualmente presentes en tu repositorio local.

- Ejemplo:
  ```
  %> bash git_ignore.sh | cat -e
  .DS_Store$
  mywork.c~$
  %>
  ```

- Para probar tu script, utilizaremos nuestro propio entorno.

## Ejercicio 07: diff

**Directorio de entrega**: `ex07/`

**Archivos a entregar**: `b`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea el archivo `b` de tal modo que:
  ```
  %>cat -e a
  STARWARS$
  Episode IV, A NEW HOPE It is a period of civil war.$
  $
  Rebel spaceships, striking from a hidden base, have won their first victory against the evil
  Galactic Empire.$
  During the battle, Rebel spies managed to steal secret plans to the Empire's ultimate weapon, the
  DEATH STAR,$
  an armored space station with enough power to destroy an entire planet.$
  $
  Pursued by the Empire's sinister agents, Princess Leia races home aboard her starship, custodian of
  the stolen plans that can save her people and restore freedom to the galaxy...$
  $
  ```

  ```
  %>diff a b > sw.diff
  ```

## Ejercicio 08: clean

**Directorio de entrega**: `ex08/`

**Archivos a entregar**: `clean`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Escriba en un archivo `clean` una línea de comandos que busque, a partir del directorio actual y en todos sus subdirectorios, los archivos cuyo nombre se termine por ~, o empiece y se termine por #.
- La línea de comandos mostrará y borrará los archivos encontrados.
- Solo se autoriza un comando: nada de ’;’ , ’&&’ ni otros trucos.

## Ejercicio 09: Illusions, not tricks, Michael...

**Directorio de entrega**: `ex09/`

**Archivos a entregar**: `ft_magic`

**Funciones autorizadas**: Ninguna

### Instrucciones
- Crea un archivo mágico que se llame `ft_magic` que tendrá que estar formateado correctamente para detectar los archivos de tipo `42 file` y constituidos por la cadena "42" en el byte 42º.

