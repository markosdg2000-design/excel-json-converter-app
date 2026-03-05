diff --git a/README.md b/README.md
index 9bef85b9b97d5f5b811e5f45085a796fe847c49b..b6ff2492022160ba85d0092852f5a1a7d97ac163 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,21 @@
-# markosdg2000-design.github.io
\ No newline at end of file
+# markosdg2000-design.github.io
+
+## Separar la app de Excel a JSON en un repositorio independiente
+
+Sí: para no mezclar esta utilidad con la web principal, conviene moverla a su propio repositorio.
+
+Este repositorio incluye un script para crear un proyecto independiente con los archivos mínimos de la app (`index.html` y `README.md`) e inicializar Git.
+
+### Uso rápido
+
+```bash
+bash scripts/create_excel_json_repo.sh ../excel-json-converter-app
+```
+
+Eso crea una carpeta nueva con:
+
+- `index.html` (app actual)
+- `README.md` (instrucciones de uso)
+- repositorio Git inicializado con commit inicial
+
+Después solo faltaría crear el repo remoto (GitHub/GitLab) y hacer `git remote add origin ...` + `git push -u origin main` desde la carpeta generada.
