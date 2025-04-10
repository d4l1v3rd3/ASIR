# YAML

## Ain't Markup Language (No es un lenguaje de marcado)

```
---
# Lista de frutas
frutas:
    - Manzana
    - Naranja
    - Fresas
    - Mango
---
````

Se pueden incluir múltiple documentos dentro de un único flujo, separándolos por tres guiones (---); los (...) indican el fin del docmuneto dentro de un flujo.

Los miembros de las listas se denotan encabezados por un guión (-) con un miembro por cada línea o entre corchetes [] y separados por ,

```
--- # Bloque
nombre : Pepe
edad : 33
--- # En línea
{nombre: Pepe, edad: 33}
```

