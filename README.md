# Lenguaje-To-Do
# 📝 Sistema de Gestión de Tareas con DSL

Un lenguaje de dominio específico (DSL) para gestionar tareas con soporte para condicionales, desarrollado como parte de un proyecto de compiladores.

## 🚀 Características

- **Gestión básica de tareas**: Agregar, completar, eliminar y mostrar tareas
- **Atributos avanzados**: Prioridad, fecha de vencimiento y etiquetas
- **Condicionales inteligentes**: Ejecutar acciones basadas en condiciones
- **Sintaxis intuitiva**: Lenguaje fácil de leer y escribir

## 📖 Sintaxis del Lenguaje

### Comandos Básicos

```todo
# Agregar tarea
task "Título" [priority N] [due "fecha"] [tag "etiqueta"]*

# Completar tarea
done "Título"

# Eliminar tarea
delete "Título"

# Mostrar tareas
show all|pending|done

# Por conteo de tareas
if count (all|pending|done) (>|<|==|!=) N acción

# Por existencia
if exists "Título" acción

# Por estado específico
if has "Título" (==|!=) (pending|done) acción
