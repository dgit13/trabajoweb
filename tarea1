Teoría
1. ¿Cómo se inicializa un repositorio local? (¿Qué comando se debe ejecutar?)
Para inicializar un repositorio local de git, se debe ejecutar:
bash
git init
Esto crea un nuevo repositorio en el directorio actual.
2. ¿Cómo hago para que un directorio deje de ser controlado por git? (¿Qué comando se debe ejecutar?)
Para dejar de controlar un directorio por git (eliminar el control de versiones), elimina la carpeta .git:
bash
rm -rf .git
Advertencia: Esto borra todo el historial y configuración de git para ese directorio.

3. Si agrego un archivo a un directorio que ya está siendo controlado por git, ¿está siendo controlado por git?
No inmediatamente. El archivo existe en el directorio, pero para que git lo controle, debes agregarlo con git add y hacer commit.

4. ¿Qué comando se utiliza para agregar un archivo al repositorio local?
bash
git add <archivo>
Ejemplo:
bash
git add sandwich.txt
5. ¿Cómo determino qué archivos fueron modificados? (¿Qué comando se debe ejecutar?)
bash
git status
Este comando muestra los archivos modificados, nuevos o eliminados.
6. ¿Qué comando se utiliza para hacer un commit?
bash
git commit -m "Mensaje del commit"
Ejemplo:
bash
git commit -m "Agrego mi sandwich.txt"
7. En tus propias palabras, ¿qué es un commit?
Un commit es como una "foto" del estado de los archivos en un momento determinado. Permite guardar los cambios realizados, con un mensaje descriptivo, para mantener un historial de versiones del proyecto.

Ejercicio Práctico
1. Crear un archivo david-falagan.txt si no existe:
bash
touch david-falagan.txt
2. Agregar a sandwich.txt condimentos e ingredientes que te gusten:
bash
echo "Pan, jamón, queso, tomate, lechuga, mayonesa" > sandwich.txt
3. Guardar el estado actual del directorio en david-falagan.txt:
bash
git status
Copia la salida y pégala en david-falagan.txt.

Explicación de git status:
Muestra los archivos nuevos, modificados o eliminados respecto al último commit. Indica qué archivos están listos para ser commiteados (staged) y cuáles no.
4. Agregar el archivo sandwich.txt al repositorio local:
bash
git add sandwich.txt
5. Explica qué cambió en la salida de git status:
Antes de git add, el archivo sandwich.txt aparecía como "Untracked" (no seguido).
Después, aparece en "staged" (preparado para commit).
6. Realizar un commit:
bash
git commit -m "Agrego mi sandwich.txt"
7. Explica qué cambió en la salida de git status:
Después del commit, git status mostrará que no hay cambios pendientes (working tree clean).

8. Agregar salsas y hacer otro commit:
bash
echo "mostaza, ketchup" >> sandwich.txt
git add sandwich.txt
git commit -m "Agrego salsas"
9. Escribir la salida de git log en juan_perez.txt y explicar:
bash
git log
Pega la salida en el archivo.
Explicación: Muestra el historial de commits, del más reciente al más antiguo.

10. Variaciones de git log:
git log --oneline: Muestra cada commit en una sola línea (hash corto + mensaje).
git log --stat: Muestra los archivos modificados y el número de líneas agregadas/eliminadas por commit.
11. Inspeccionar diferencias entre commits:
bash
git diff
Muestra los cambios no commiteados.
Para comparar dos commits:

bash
git diff <hash1> <hash2>
Explica que muestra las diferencias línea por línea.

En Windows:
bash
git difftool --tool=meld <hash>
En Linux:
bash
git difftool --tool=opendiff <hash>
12. Crear un archivo sandwich2.txt en la carpeta 1.commit:
bash
mkdir -p 1.commit
echo "pan, pollo, tomate" > 1.commit/sandwich2.txt
13. Agregar el archivo al repositorio:
bash
git add 1.commit/sandwich2.txt
git commit -m "Agrego sandwich2.txt"
14. Renombrar el archivo:
bash
git mv 1.commit/sandwich2.txt 1.commit/sandwich2_feo.txt
git commit -m "Renombro sandwich2.txt a sandwich2_feo.txt"
Explicación:

Antes del commit, git status muestra el archivo como "renombrado".
Después del commit, el cambio queda registrado y el log muestra el nuevo commit.
15. Borrar el archivo:
bash
git rm 1.commit/sandwich2_feo.txt
git commit -m "Borro sandwich2_feo.txt"
Explicación:

Antes del commit, git status muestra el archivo como "deleted".
Después del commit, el log muestra el commit de borrado.
16. Inspeccionar la bitácora:
bash
git log --stat
Explicación:
Muestra los commits y, para cada uno, los archivos modificados y las líneas añadidas o eliminadas.
