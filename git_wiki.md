# 🚀 Flujo común de trabajo con Git y GitHub

Este flujo se utiliza para desarrollar nuevas funcionalidades o correcciones en un proyecto, manteniendo limpio el historial con **Squash Merge**.

---

## 1️⃣ Crear una nueva rama
Usa un nombre descriptivo para la tarea o funcionalidad.
```bash
git checkout -b nombre-de-rama
````

---

## 2️⃣ Hacer cambios en el código

Edita, agrega o elimina archivos según lo que requiera la tarea.

---

## 3️⃣ Añadir cambios al *staging area*

```bash
git add .
# o para agregar un archivo específico:
git add ruta/archivo
```

---

## 4️⃣ Crear un commit

Usa mensajes claros y en presente.

```bash
git commit -m "feat: descripción corta del cambio"
```

---

## 5️⃣ Subir la rama al repositorio remoto

```bash
git push -u origin nombre-de-rama
```

---

## 6️⃣ Abrir un Pull Request (PR)

En GitHub:

1. Selecciona `base: main` y `compare: nombre-de-rama`.
2. Agrega título y descripción.
3. Solicita revisión si es necesario.

---

## 7️⃣ Realizar **Squash Merge**

En GitHub:

* Opción **Squash and Merge**: combina todos los commits de la rama en **uno solo** en `main`.
* Ventajas:

  * Historial limpio.
  * Fácil de revertir.

---

## 8️⃣ Cambiar a `main` localmente

```bash
git checkout main
```

---

## 9️⃣ Actualizar la rama `main`

```bash
git pull
```

---

✅ **Consejo:** Borra la rama local y remota después de mergear para mantener el repositorio ordenado:

```bash
git branch -d nombre-de-rama         # Local
git push origin --delete nombre-de-rama  # Remoto
```


