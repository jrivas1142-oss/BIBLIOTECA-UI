

STEFYMAKEUP |Biblioteca UI: Biblioteca de Componentes UI Avanzados

NOMBRES: JULEXI ESTEFANIA RIVAS RISCO 
*Materia:* Desarrollo de Sistemas Informáticos
*Objetivo:* Diseñar y desarrollar una biblioteca de componentes de interfaz de usuario (UI)
reutilizables utilizando técnicas de CSS avanzado, con el fin de fomentar la
modularidad, reutilización, coherencia visual y escalabilidad en el desarrollo de
sitios y aplicaciones web.

**Estructura del Proyecto y Modularidad**

El proyecto cumple con la modularidad requerida al separar los estilos en archivos específicos para cada componente, siguiendo la convención BEM.


**Cómo Importar los Estilos**
Para utilizar la biblioteca, solo es necesario enlazar el archivo `main.css` en la cabecera del documento html

html
<link rel="stylesheet" href="styles/main.css">

**Guía de Estilos y Uso de CSS Avanzado**
# Variables Globales

El diseño es controlado por variables CSS, lo que facilita el cambio de la paleta de colores de forma centralizada.
# :root {
  /* Paleta de Colores*/
  --color-primary: #240046;   
  --color-secondary: #6d597a; 
  --color-danger: #b56576;
  --color-text: #212121;      
  --color-background: #f7ede2;
  --color-white: #e0aaff;     
  
  /* Tipografía*/
  --font-family-base: 'Lato', sans-serif;
  --font-family-heading: 'Montserrat', sans-serif;
  --font-size-base: 16px;
  
  /* Espaciado */
  --spacing-sm: 8px;
  --spacing-md: 16px;
  --spacing-lg: 32px; 
  
  /* Bordes y Sombras */
  --border-radius-base: 4px;
  --shadow-sm: 0 4px 6px rgba(0, 0, 0, 0.08); 
} 

**Componentes UI Funcionales**
# Navbar Responsivo (.navbar)
Barra de navegación adaptable que colapsa en un menú hamburguesa en dispositivos móviles.
Uso Avanzado: Flexbox y Media Queries
---------------------------------------------------------------------------------------------
# Botones (.btn)
Implementación de la convención BEM con clases base y modificadores para estilo y tamaño.
Uso Avanzado: Transiciones en background-color y box-shadow al pasar el mouse.
Ejemplo: <button class="btn btn--primary btn--large">Ver coleccion</button>
-----------------------------------------------------------------------------------
# Tarjetas de Producto y CSS Grid (.card, .card-grid)
Un contenedor (.card-grid) que utiliza CSS Grid para mostrar tarjetas (.card) en un diseño de columnas fluido.
Uso Avanzado: display: grid; con auto-fit y minmax para total adaptabilidad.
-------------------------------------------------------------------------------------
# Formularios de Contacto (.form-group)
Componentes para la entrada de datos (email, mensaje).
Uso Avanzado: Uso de :focus en el input y textarea para resaltar el campo activo con el color primario
Ejemplo:
<div class="form-group">   
 <label for="email" class="form-label">Email</label>
 <input type="email" class="form-input">
</div>
--------------------------------------------------------------------------

# Acordeón (FAQ)
Sección de Preguntas Frecuentes interactiva que se expande y colapsa al hacer clic.
Uso Avanzado (Crítico): Se controla exclusivamente con CSS mediante la pseudo-clase :checked y la animación de la propiedad max-height.
---------------------------------------------------------------------------------------
# Hero Section (.hero-section)
Banner principal de la página, centrado y con alineación controlada.
Uso Avanzado: Flexbox para centrar contenido tanto vertical como horizontalmente.