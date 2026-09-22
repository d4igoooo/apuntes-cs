## Jerarquía de títulos (Encabezados)

- Para estructurar documentos (dejar un espacio al lado después de los `#`)

```
# Título 1 (H1) - Tema principal
## Título 2 (H2) - Secciones clave
### Título 3 (H3) - Subsecciones
#### Título 4 (H4) - Divisiones menores
##### Título 5 (H5)
###### Título 6 (H6)
```

---
## Formatos básicos de texto

- Destacar términos, enfatizar.

```
**Texto en negrita**
*Texto en cursiva* o _cursiva_
***Texto en negrita y cursiva***
~~Texto tachado~~
==Texto resaltado en amarillo (función nativa de Obsidian)==
```

> [!TIP] Resultados
> **Texto en negrita**
*Texto en cursiva* o _cursiva_
***Texto en negrita y cursiva***
~~Texto tachado~~
==Texto resaltado en amarillo (función nativa de Obsidian)==

---
## Enlaces entre notas

- Para gráfico y conexión de ideas en Obsidian

```
# Enlace directo a otra nota
[[Nombre de la nota]]

# Enlace con texto alternativo (alias en el texto)
[[Nombre de la nota|Texto visible personalizado]]

# Enlace directo a un encabezado interno de otra nota
[[Nombre de la nota#Nombre de la sección]]

# Enlace directo a un bloque específico de texto
[[Nombre de la nota#^identificador-de-bloque]]

# Incrustar el contenido completo de otra nota dentro de esta
![[Nombre de la nota]]

# Enlace externo tradicional a la web
[Texto del enlace](https://direccion-web.com)
```

> [!TIP] Resultados
> - Enlace directo a otra nota
[[Nombre de la nota]]
> - Enlace con texto alternativo (alias en el texto)
[[Nombre de la nota|Texto visible personalizado]]
> - Enlace directo a un encabezado interno de otra nota
[[Nombre de la nota#Nombre de la sección]]
> - Enlace directo a un bloque específico de texto
[[Nombre de la nota#^identificador-de-bloque]]
> - Incrustar el contenido completo de otra nota dentro de esta
![[Nombre de la nota]]
> - Enlace externo tradicional a la web
[Texto del enlace](https://direccion-web.com)

---
## Listas y casillas (Tareas)

 - Desglosar conceptos, secuencias de pasos, seguimiento de pendientes

```
# Lista sin orden (viñetas)
- Elemento de lista
  - Sub-elemento (con tabulador)

# Lista ordenada
1. Primer paso
2. Segundo paso
3. Tercer paso

# Casillas de verificación / To-Do
- [ ] Tarea pendiente
- [x] Tarea completada
```

> [!TIP] Lista sin orden (viñetas)
> - Elemento de lista
> 	- Sub-elemento (con tabulador)

> [!TIP] Lista ordenada
> 1. Primer paso
> 2. Segundo paso
> 3. Tercer paso

> [!TIP] Casillas de verificación / To-Do
> - [ ] Tarea pendiente
> - [x] Tarea completada

---
## Bloques de código y comandos

- Para comandos de terminal, snippets de Java, SQL, etc.

````
# Código en línea (inline)
Usa el comando `git status` para ver el estado.

# Bloque de código con resaltado de sintaxis (especificando lenguaje luego del primer ```)
```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("Hola, desarrollo backend");
    }
}
```

```bash
git add .
git commit -m "feat: nueva funcionalidad"
```

```sql
SELECT id, nombre, email FROM usuarios WHERE activo = true;
```
````

> [!TIP] Java
> ```java
> public class HolaMundo {
> 	public static void main(String[] args) {
> 		System.out.println("Hola, desarrollo backend");
> 	}
> }
> ```

> [!TIP] Bash
> ```bash
> git add .
> git commit -m "feat: nueva funcionalidad"
> ```

> [!TIP] SQL
> ```sql
> SELECT id, nombre, email FROM usuarios WHERE activo = true;
> ```

---
## Citas y bloques de notas

- Para definiciones breves, advertencias o aclaraciones.

```
> Ejemplo de cita en bloque de MD
```

>[!TIP] Resultado
> Ejemplo de cita en bloque de MD

---
## Callouts

- Cajas decorativas para resaltar conceptos, advertencias o consejos.

```
> [!NOTE]
> Nota informativa o recordatorio general.

> [!TIP]
> Consejo práctico o buenas prácticas.

> [!WARNING]
> Advertencia de error o comando peligroso.

> [!INFO]
> Contexto adicional.
```

> [!NOTE]
> Nota informativa o recordatorio general.

> [!TIP]
> Consejo práctico o buenas prácticas.

> [!WARNING]
> Advertencia de error o comando peligroso.

> [!INFO]
> Contexto adicional.

---
## Tablas comparativas

- Para comparar tecnologías, métodos o estructuras de datos (como `ArrayList` vs `LinkedList`).

```
| Herramienta | Caso de uso principal | Ventaja |
| :--- | :--- | :--- |
| **`git init`** | Repositorios locales existentes | Control total inicial |
| **`git clone`** | Proyectos nuevos o remotos | Trae ramas y origin listo |
```

> [!TIP] Resultado
> | Herramienta | Caso de uso principal | Ventaja |
| :--- | :--- | :--- |
| **`git init`** | Repositorios locales existentes | Control total inicial |
| **`git clone`** | Proyectos nuevos o remotos | Trae ramas y origin listo |

---
## Separadores temáticos y comentarios

- Para cortar visualmente secciones largas o dejar anotaciones que no se ven en vista de lectura.

```
# Línea divisoria horizontal
---

# Comentarios ocultos (solo visibles en el editor de Obsidian, invisibles en lectura)
%% Comentario oculto que NO se muestra al exportar o leer %%
```
 
 %% Comentario oculto %%

