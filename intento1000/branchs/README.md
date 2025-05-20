¡Claro! Aquí tienes respuestas breves y directas para la parte teórica (2.1) y un resumen de los comandos a utilizar en la parte práctica (2.2):

---

## 2.1. Preguntas

1. **¿Qué es un branch?**  
   Un branch (rama) es una línea paralela de desarrollo en un repositorio Git, que permite trabajar en cambios sin afectar la rama principal.

2. **¿Por qué pueden ser útiles los branches?**  
   Permiten desarrollar nuevas características, corregir errores o experimentar sin alterar el código principal, facilitando el trabajo en equipo y la organización.

3. **¿Cómo se crea una branch?**  
   ```bash
   git branch nombre_rama
   ```

4. **¿Cómo se cambia a una branch?**  
   ```bash
   git checkout nombre_rama
   ```

5. **¿Cómo se elimina una branch?**  
   ```bash
   git branch -d nombre_rama
   ```

6. **¿Cómo se crea una branch y se cambia a ella en un solo paso?**  
   ```bash
   git checkout -b nombre_rama
   ```

7. **¿Qué es un merge?**  
   Es la acción de combinar los cambios de una rama con otra.

8. **¿Cómo se realiza un merge?**  
   Primero cambia a la rama donde quieres combinar, luego ejecuta:
   ```bash
   git merge nombre_rama
   ```

9. **¿Qué es un tag?**  
   Un tag es una referencia que apunta a un punto específico en la historia del repositorio, normalmente usado para marcar versiones.

10. **¿Cómo se crea un tag?**  
    ```bash
    git tag -a nombre_tag -m "mensaje"
    ```

---

## 2.2. Ejercicio Práctico (Resumen de comandos)

1. Crear branch `experimento`:
   ```bash
   git branch experimento master
   ```
2. Cambiar a `experimento`:
   ```bash
   git checkout experimento
   ```
3. Ver en qué branch estás:
   ```bash
   git branch
   ```
4. Editar `2.branchs/pizza.txt` (agregar albahaca arriba del queso) y guardar cambios.
5. Hacer commit:
   ```bash
   git add 2.branchs/pizza.txt
   git commit -m "Agregar albahaca arriba del queso"
   ```
6. Editar de nuevo (agregar orégano arriba de la albahaca) y hacer commit:
   ```bash
   git add 2.branchs/pizza.txt
   git commit -m "Agregar orégano arriba de la albahaca"
   ```
7. Ver el grafo:
   ```bash
   git graph
   ```
8. Cambiar a `master`:
   ```bash
   git checkout master
   ```
9. Crear y cambiar a branch `anana`:
   ```bash
   git checkout -b anana
   ```
10. Editar (agregar anana debajo del queso) y commit:
    ```bash
    git add 2.branchs/pizza.txt
    git commit -m "Agregar anana debajo del queso"
    ```
11. Ver el grafo:
    ```bash
    git graph
    ```
12. Cambiar a `master`:
    ```bash
    git checkout master
    
13. Agregar cebolla debajo de la salsa y commit:
    bash
    git add 2.branchs/pizza.txt
    git commit -m "Agregar cebolla debajo de la salsa"
    
14. Ver el grafo:
    bash
    git graph

15. Merge de `anana` en `master`:
    bash
    git merge anana
    git graph
    ```
16. Ver ramas mergeadas:
    ```bash
    git branch --merged
    ```
17. Merge de `experimento` en `master`:
    ```bash
    git merge experimento
    git graph
    ```
18. (Si hubo conflicto, Git te lo indicará; si no, lo hizo automáticamente).

19. Ver ramas mergeadas:
    ```bash
    git branch --merged
    ```
20. Eliminar branches:
    ```bash
    git branch -d anana
    git branch -d experimento
    ```
21. Ver ramas mergeadas:
    ```bash
    git branch --merged
    ```
22. Ver el grafo:
    ```bash
    git graph
    ```
23. Crear tag `pizza` en el último commit:
    ```bash
    git tag -a pizza -m "Receta de la pizza."
    ```
24. Ver tags:
    ```bash
    git tag
    ```
25. Ver detalles del tag:
bash
    git show pizza


