# Intento_Parcial

Apoyo Parcial

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

--------------------------------------------------------------------------------
Console.WriteLine("Hello, World!");

Personas persona = new Personas();
var persona1 = new Personas();
Estudiantes persona2 = new Estudiantes();
Personas persona3 = persona2;
Personas persona4 = (Personas)persona2;
Personas persona5 = (Estudiantes)persona2;

persona.Id = 1;
persona.Nombre = "Pepito Perez";
persona.Estatura = 1.60m;
persona.Vive = false;
persona.Fecha = DateTime.Now;
persona.Estado = new Estados() { Id = 1, Nombre = "Viudo" };
persona.VideoJuegos = new List<VideoJuegos>();
persona.VideoJuegos.Add(new VideoJuegos() { Id = 1, Nombre = "GTA" });
persona.VideoJuegos.Add(new VideoJuegos() { Id = 2, Nombre = "DOOM" });

Console.WriteLine(persona.Nombre);
Console.WriteLine(persona.Estado.Nombre);

foreach (var elemento in persona.VideoJuegos)
{
    Console.WriteLine(elemento.Nombre);
}

public class Estados
{
    public int Id;
    public string? Nombre;
}

public class VideoJuegos
{
    public int Id;
    public string? Nombre;
}

public class Personas
{
    public int Id;
    public string? Nombre;
    public decimal Estatura;
    public bool Vive;
    public DateTime Fecha;
    public Estados? Estado;
    public List<VideoJuegos>? VideoJuegos;
}

public class Estudiantes : Personas
{
    public string? Carnet;
}
--------------------------------------------------------------------------------