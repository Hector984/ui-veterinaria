📌 Cómo Mantener Tu Fork Actualizado

Si hiciste un fork de un repositorio y quieres mantenerlo sincronizado con el original, sigue estos pasos.

🔄 Actualizar tu fork con los cambios del repositorio original

1️⃣ Abrir la terminal y navegar al repositorio local

cd ruta/de/tu/repositorio

2️⃣ Descargar los cambios más recientes del upstream

git fetch upstream

3️⃣ Cambiar a la rama `` antes de fusionar

git checkout main

4️⃣ **Fusionar los cambios del upstream en tu **``

git merge upstream/main

5️⃣ Subir los cambios actualizados a tu fork en GitHub

git push origin main

⚡ **(Opcional) Probar los cambios antes de aplicarlos en **``

Si quieres revisar los cambios antes de aplicarlos a tu rama principal, sigue estos pasos:

1️⃣ Crear una rama de pruebas:

git checkout -b test-updates

2️⃣ Fusionar los cambios en esta rama:

git merge upstream/main

3️⃣ Si todo funciona bien, aplicar los cambios en main:

git checkout main
git merge test-updates
git push origin main