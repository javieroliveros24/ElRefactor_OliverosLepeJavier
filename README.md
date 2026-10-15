Taller Practico DIW (RA2): "El Refactor"Este proyecto consiste en la refactorizacion integral de un sitio web personal tipo portfolio de 3 paginas (index.html, sobre.html y contacto.html). Se ha transformado un codigo heredado con mala arquitectura en un sitio moderno, mantenible y 100% semantico mediante el uso de HTML5 y SASS (SCSS).Resumen del Trabajo RealizadoLimpieza del Codigo HTML (Refactorizacion):Se eliminaron todos los atributos style="..." en linea (index.html).Se elimino el bloque <style>...</style> interno (sobre.html).Se reestructuro todo el HTML para eliminar el uso innecesario de etiquetas <div>, sustituyendolas por etiquetas semanticas de HTML5 (<header>, <nav>, <main>, <section>, <article>, <footer>, etc.).Modularizacion con SASS:Se creo una arquitectura modular utilizando parciales SCSS (ficheros que empiezan con _).Se declararon variables para controlar la paleta de colores y las fuentes tipograficas en un unico lugar.Se uso anidamiento (nesting) y Flexbox para maquetar la navegacion y los elementos de forma ordenada.Inclusion de la Pagina de Contacto:Se creo la tercera pagina contacto.html con un formulario estructurado y estilizado.Validacion y Calidad:El archivo compilado css/estilos.css supero la validacion del W3C CSS Validator sin errores.Estructura del Proyectoproyecto-refactorizado/
├── css/
│   └── estilos.css         # Archivo CSS generado automaticamente por Live Sass
├── scss/
│   ├── _variables.scss     # Paleta de colores y tipografia de Google Fonts
│   ├── _global.scss        # Reset basico y estilos generales del cuerpo
│   ├── _header.scss        # Cabecera y menu de navegacion con Flexbox
│   ├── _formularios.scss   # Estilos para el formulario de contacto
│   ├── _footer.scss        # Estilos para el pie de pagina
│   └── estilos.scss        # Archivo principal de SASS que importa los parciales
├── index.html              # Pagina principal de Inicio (Semantica, sin <div>)
├── sobre.html              # Pagina "Sobre mi" (Semantica, sin <div>)
├── contacto.html           # Pagina de Contacto (Semantica, sin <div>)
└── README.md               # Documentacion del proyecto
Identidad Visual y Paleta de ColoresPara el rediseno se sustituyeron los colores por defecto por una paleta personalizada:Elemento / UsoVariable SASSColor (HEX)Color Primario (Header, Footer, Botones)$color-primario#0A4F60Color Secundario (Hover en menu y botones)$color-secundario#2A9D8FTexto Principal$color-texto#2B2D42Fondo de la web$color-fondo#F8F9FAFondo Tarjetas/Formularios$color-blanco#FFFFFFTipografiaEncabezados (h1, h2, h3): 'Montserrat', sans-serif.Cuerpo de texto (p, input, etc.): 'Roboto', sans-serif.
(Importadas dinamicamente desde Google Fonts en _variables.scss).Pasos para Trabajar con el ProyectoClonar el repositorio:git clone https://github.com/tu-usuario/proyecto-refactorizado.git
Abrir en VS Code:
Abre la carpeta del proyecto en Visual Studio Code.Compilar SASS:Asegurate de tener instalada la extension Live Sass Compiler (Glen Marks).Haz clic en el boton Watch Sass situado en la barra inferior para vigilar los cambios en scss/ y actualizar css/estilos.css automaticamente.Visualizar la web:
Abre index.html en tu navegador o mediante la extension Live Server.Verificacion W3CEl archivo css/estilos.css fue verificado en el W3C CSS Validator por entrada directa, obteniendo un resultado correcto sin ningun tipo de error o advertencia.
