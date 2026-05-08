Catálogo de Videojuegos - ASP.NET Core MVCEste proyecto es una aplicación web desarrollada con ASP.NET Core MVC diseñada para gestionar un catálogo de videojuegos. Cuenta con una estética personalizada inspirada en los Salamanders de Warhammer 40K, combinando funcionalidad técnica con un diseño visual temático.👤 Datos del EstudianteCampoInformaciónNombre[Tu Nombre]Matrícula[Tu Matrícula]Universidad[Nombre de la Universidad]Profesor[Nombre del Profesor]Materia[Nombre de la Materia]TareaCatálogo de Videojuegos con MVC📝 Descripción GeneralLa aplicación permite visualizar una lista de videojuegos, consultar detalles específicos, filtrar por género y registrar nuevos títulos mediante formularios. El enfoque principal fue el dominio del patrón Modelo-Vista-Controlador (MVC) y la manipulación de archivos estáticos para una personalización profunda.🎨 Temática: Salamanders (Warhammer 40K)El diseño visual utiliza:Colores: Verdes esmeralda, naranjas de fuego y negros volcánicos.Texturas: Fondos con estética de forja y lava.Interactividad: Animaciones suaves y sombras brillantes para una experiencia moderna.🚀 Tecnologías UtilizadasLenguaje: C#Framework: ASP.NET Core MVCFrontend: Razor Views, HTML5, CSS3, Bootstrap, JavaScriptHerramientas: Visual Studio, Git, GitHub📂 Estructura del ProyectoPlaintextCatalogo/
├── Controllers/         # Lógica de navegación y control
├── Models/              # Definición de datos (Item, ErrorViewModel)
├── Views/               # Vistas Razor (Index, Detalle, Agregar, Layout)
├── wwwroot/             # Archivos estáticos
│   ├── css/             # Estilos personalizados (site.css)
│   ├── images/          # Assets visuales (salamanders-bg, forge-texture)
│   └── js/              # Scripts de cliente
├── Program.cs           # Configuración de la aplicación
└── Catalogo.csproj      # Archivo de proyecto
⚙️ FuncionalidadesVisualizar Catálogo: Tarjetas con título, género, consola, año y descripción.Filtrado Dinámico: Botones para segmentar juegos por categoría.Detalles Extendidos: Vista dedicada para profundizar en la información de cada registro.Registro de Juegos: Formulario funcional para añadir nuevos elementos al catálogo.🛠️ Comandos de UsoDesarrollo con .NETBash# Restaurar dependencias
dotnet restore

# Compilar proyecto
dotnet build

# Ejecutar la aplicación
dotnet run

# Limpiar archivos temporales
dotnet clean
Gestión con GitBash# Inicializar y preparar archivos
git init
git add .

# Crear commit
git commit -m "Proyecto catalogo de videojuegos ASP.NET Core MVC"

# Subir a GitHub
git remote add origin URL_DEL_REPOSITORIO
git push -u origin main
🖌️ Personalización y DiseñoManejo de ImágenesLas imágenes se sirven desde wwwroot/images/ y se integran en el CSS mediante rutas relativas:CSS/* Ejemplo de fondo con textura volcánica */
.main-container {
    background: linear-gradient(rgba(10, 12, 15, 0.62), rgba(10, 12, 15, 0.76)),
                url('/images/forge-texture.jpg') center / cover no-repeat;
}
Paleta de Colores (Salamanders Theme)Negro Volcánico: #0b0d0fVerde Esmeralda: #2e8b57Naranja Fuego: #ff7a1aTexto Claro: #f3f0e8Animaciones CSSSe implementaron efectos de entrada y pulsación para mejorar el feedback visual:CSS@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(18px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
🧠 Aprendizajes y RetosEstructura MVC: Comprensión profunda del flujo de datos entre Modelos, Vistas y Controladores.Archivos Estáticos: Configuración de wwwroot para servir recursos de diseño sin conflictos de rutas.UX/UI: Balancear una temática visual intensa (Warhammer 40K) con la legibilidad y usabilidad de la interfaz.Reutilización: Aplicación de conceptos de cuatrimestres anteriores (HTML/Bootstrap) adaptados a un entorno de servidor robusto.📈 Mejoras Futuras[ ] Integración con base de datos SQL Server/Entity Framework.[ ] Sistema de autenticación de usuarios.[ ] Implementación de CRUD completo (Editar/Eliminar).[ ] Buscador en tiempo real por título.[ ] Paginación para catálogos extensos.🏁 ConclusiónEste proyecto representa la integración de lógica de backend con diseño creativo. No solo cumple con los requisitos funcionales de un catálogo de videojuegos, sino que demuestra la capacidad de personalizar entornos de trabajo profesionales en ASP.NET Core para crear productos únicos y atractivos.
