# CLI User Manager

Aplicación de línea de comandos (CLI) construida con Node.js para realizar operaciones CRUD (Crear, Leer, Actualizar, Borrar) sobre un sistema de usuarios.

---

##  Requisitos previos

- **Node.js** instalado en tu sistema.
- Proyecto configurado (haber ejecutado `npm install` si tenés dependencias en `package.json`).

---

##  Instalación

1. Cloná el repositorio o descargá los archivos.
2. Abrí la terminal en la carpeta del proyecto.
3. Asegurate de tener el archivo `controllers.js` correctamente configurado.

---

## Uso

La sintaxis general es:

```bash
node index.js <operacion> [argumentos...]
```

### Tabla de comandos

| Operación | Descripción              | Argumentos necesarios          |
|-----------|--------------------------|-------------------------------|
| `get`     | Lista todos los usuarios | Ninguno                        |
| `add`     | Crea un nuevo usuario    | `nombre`, `email`, `password`  |
| `update`  | Actualiza un usuario     | `nombre`, `email`, `password`, `id` |
| `delete`  | Elimina un usuario       | `id`                           |

---

##  Ejemplos de uso

#### 1. Obtener usuarios

```bash
node index.js get
```

#### 2. Agregar un usuario

```bash
# Sintaxis
node index.js add <nombre> <email> <password>

# Ejemplo
node index.js add "Juancito" "juan@gmail.com" "megustaelddl"
```

#### 3. Actualizar un usuario

```bash
# Sintaxis
node index.js update <nombre> <email> <password> <id>

# Ejemplo
node index.js update "Juan Actualizado" "juan.nuevo@gmail.com" "password123" 1
```

#### 4. Eliminar un usuario

```bash
# Sintaxis
node index.js delete <id>

# Ejemplo
node index.js delete 1
```