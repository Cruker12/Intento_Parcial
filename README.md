# Intento_Parcial

// Prueba de commit desde Visual Studio (1)
// Estas en la RamaP1, Hola:3

git clone URL                    # Clona un repositorio remoto a tu máquina  
git fetch                        # Descarga actualizaciones del remoto sin fusionarlas  
git pull                         # Descarga actualizaciones y las fusiona con tu rama actual  

git add *                        # Añade todos los archivos modificados al staging  
git commit -am "Descripcion"     # Crea un commit con cambios (añade y guarda con mensaje)  
git push                         # Sube los commits locales al repositorio remoto  

git branch dev1                  # Crea una nueva rama llamada dev1  
git checkout dev1                # Cambia a la rama dev1  
git push -u origin dev1          # Sube la rama dev1 al remoto y la enlaza (tracking)  
git push origin HEAD:main        # Sube tu rama actual (HEAD) al remoto como main  

git checkout -- .                # Descarta todos los cambios locales no guardados  
