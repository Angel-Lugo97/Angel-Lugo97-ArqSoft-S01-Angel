# Catálogo de Videojuegos - ASP.NET Core MVC

Este proyecto es una aplicación web desarrollada con **ASP.NET Core MVC** diseñada para gestionar un catálogo de videojuegos. Cuenta con una estética personalizada inspirada en los **Salamanders de Warhammer 40K**, combinando funcionalidad técnica con un diseño visual temático.

---

## 👤 Datos del Estudiante

| Campo | Información |
| :--- | :--- |
| **Nombre** | [Tu Nombre] |
| **Matrícula** | [Tu Matrícula] |
| **Universidad** | [Nombre de la Universidad] |
| **Profesor** | [Nombre del Profesor] |
| **Materia** | [Nombre de la Materia] |
| **Tarea** | Catálogo de Videojuegos con MVC |

---

## 📝 Descripción General

La aplicación permite visualizar una lista de videojuegos, consultar detalles específicos, filtrarlos por género y registrar nuevos títulos mediante formularios. El enfoque principal fue el dominio del patrón **Modelo-Vista-Controlador (MVC)**.

### 🎨 Temática: Salamanders (Warhammer 40K)
El diseño visual utiliza:
* **Colores:** Verdes esmeralda, naranjas de fuego y negros volcánicos.
* **Texturas:** Fondos con estética de forja y lava.
* **Interactividad:** Animaciones suaves y sombras brillantes.

---

## 🚀 Tecnologías Utilizadas

* **Lenguaje:** C#
* **Framework:** ASP.NET Core MVC
* **Frontend:** Razor Views, HTML5, CSS3, Bootstrap, JavaScript
* **Herramientas:** Visual Studio, Git, GitHub

---

## 📂 Estructura del Proyecto

```text
Catalogo/
├── Controllers/         # Lógica de navegación y control
├── Models/              # Definición de datos
├── Views/               # Vistas Razor
├── wwwroot/             # Archivos estáticos
│   ├── css/             # Estilos personalizados
│   ├── images/          # Assets visuales
│   └── js/              # Scripts de cliente
├── Program.cs           # Configuración
└── Catalogo.csproj      # Archivo de proyecto
⚙️ Funcionalidades
Visualizar Catálogo: Tarjetas con título, género, consola, año y descripción.

Filtrado Dinámico: Botones para segmentar juegos por categoría.

Detalles Extendidos: Vista dedicada para profundizar en la información.

Registro de Juegos: Formulario funcional para añadir nuevos elementos.

🛠️ Comandos de Uso
Desarrollo con .NET
Bash
# Restaurar dependencias
dotnet restore

# Compilar proyecto
dotnet build

# Ejecutar la aplicación
dotnet run
Gestión con Git
Bash
# Inicializar y preparar archivos
git init
git add .

# Crear commit
git commit -m "Proyecto catalogo de videojuegos ASP.NET Core MVC"

# Subir a GitHub
git remote add origin URL_DEL_REPOSITORIO
git push -u origin main
🖌️ Personalización y Diseño
Manejo de Imágenes
Las imágenes se sirven desde wwwroot/images/ y se integran en el CSS mediante rutas relativas:

CSS
.main-container {
    background: linear-gradient(rgba(10, 12, 15, 0.62), rgba(10, 12, 15, 0.76)),
                url('/images/forge-texture.jpg') center / cover no-repeat;
}
Animaciones CSS
Se implementaron efectos de entrada para mejorar el feedback visual:

CSS
@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(18px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
📈 Mejoras Futuras
[ ] Integración con base de datos SQL Server.

[ ] Sistema de autenticación de usuarios.

[ ] Implementación de CRUD completo (Editar/Eliminar).

[ ] Buscador en tiempo real por título.

🏁 Conclusión
Este proyecto representa la integración de lógica de backend con diseño creativo. Demuestra la capacidad de personalizar entornos profesionales en ASP.NET Core para crear productos únicos.


**Tip:** Asegúrate de que el archivo en el que pegas esto tenga la extensión `.md` (ejemplo: `README.md`). Si usas el editor de GitHub directamente, usa la pestaña **"Edit"** para pegar el código y luego revisa en **"Preview"** que se vea bien.
