1. Instalar git flow en Arch:  
yay gitflow-avh  

2. Configurar git flow globalmente para usar 'main' como la rama principal:  
git config --global gitflow.branch.master main  

3. Inicializar git flow en un nuevo repositorio:  
git flow init (-d para aplicar opciones por defecto)  
git add LICENSE README.md  
git commit -m "LICENSE y README.md iniciales"  
