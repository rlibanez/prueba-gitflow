1. Instalar git flow en Arch:  
yay gitflow-avh  
  
2. Configurar git flow globalmente para usar 'main' como la rama principal:  
git config --global gitflow.branch.master main  
  
3. Inicializar git flow en un nuevo repositorio:  
git flow init (-d para aplicar opciones por defecto)  
git add LICENSE README.md  
git commit -m "LICENSE y README.md iniciales"  
  
4. Crear una nueva feature (funcionalidad):  
git flow feature start helloworld  
git add hello.py  
git commit -m "Añadir script de saludo"  
git flow feature finish helloworld (elimina la rama feature/helloworld)  
git flow feature finish -k helloworld (mantiene la rama feature/helloworld)  
  
5. Crear una nueva release (versión):  
git flow release start 1.0.0  
git add version.py  
git commit -m "Preparar la versión 1.0.0"  
git flow release finish 1.0.0 (elimina la rama release/1.0.0)  
git flow release finish -k 1.0.0 (mantiene la rama release/1.0.0)  
  
6. Crear un nuevo hotfix (bug en producción):  
git flow hotfix start fix-bug8071  
git add bug8071.py  
git commit -m "Corregir bug 8071"  
git flow hotfix finish -k fix-bug  
  

7. Para ver el estado actual de las ramas:  
git flow feature  
git flow release  
git flow hotfix  
  