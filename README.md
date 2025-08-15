VisorVB 🌍
  
VisorVB is a multipurpose, web-based map viewer built with Leaflet, designed to integrate multiple WMS services (e.g., PNOA from IGN Spain) with customizable transparency and opacity. It offers an interactive interface with a customizable toolbar, circular navigation controls, and support for GeoJSON overlays. This project is ideal for geospatial enthusiasts and developers. 🗺️

📋 Table of Contents

Features
Installation
Usage
Customization
Contributing
License
Español


Features 🚀

Multi-WMS Support: Seamlessly integrate multiple WMS services (e.g., PNOA) with adjustable transparency and opacity for layered visualization. 🛰️
Interactive Navigation: Circular navigation pad (bottom-right) for panning and centering the map. 🎮
Dynamic Coordinates: Toggle coordinates and zoom level display with the 'C' key (bottom-left). 📍
Customizable Toolbar: Expandable toolbar (top-left) for adding custom tools and functionalities. 🛠️
GeoJSON Integration: Easily overlay parcel data or other geospatial layers via GeoJSON. 📊
Responsive Design: Adapts to 100% of the parent container's width for a seamless experience. 📱💻


Installation 🔧

Clone the Repository:
git clone https://github.com/RubenBarrionuevo/VisorVB.git


Open the Project:

Open index.html directly in a modern web browser (Chrome, Firefox, etc.)—no server required.
Optionally, serve the project locally (e.g., with Python):python -m http.server 8000

Then navigate to http://localhost:8000.


Dependencies:

Uses CDN-hosted Leaflet (v1.9.4) and Font Awesome (v6.0.0) for icons. No additional installation needed. 🌐




Usage 🖱️

Open the Map:

Initializes centered on Punta Chullera, Manilva (coordinates: 36.3217, -5.2489, zoom level 17).


Navigation:

Use the circular navigation pad (bottom-right) to pan (up, down, left, right) or center the map. 🧭
Drag the map or use the mouse wheel for zooming.


Coordinates Display:

Press the 'C' key to toggle the display of current coordinates and zoom level (bottom-left). 📍


Toolbar:

Click the tools icon (top-left) to open the customizable toolbar, currently featuring a test button. 🛠️


Add WMS Layers:

Modify the L.tileLayer.wms calls in index.html to add additional WMS services. Adjust opacity and transparent parameters for layering. 🛰️
Example: Add a new WMS layer with L.tileLayer.wms('WMS_URL', { layers: 'LAYER_NAME', format: 'image/png', transparent: true, opacity: 0.5 }).


Add GeoJSON:

Update the parcelsGeoJSON variable or load a .geojson file to overlay custom data. 📊




Customization 🎨

WMS Layers: Add multiple WMS services by extending the JavaScript code with additional L.tileLayer.wms instances. Use the opacity (0.0 to 1.0) and transparent: true options to control layer visibility.
GeoJSON Layers: Modify parcelsGeoJSON in index.html or use the commented fetch code to load external GeoJSON files.
Toolbar Options: Extend the L.Control.Tools panel in the JavaScript code to add new buttons or functionalities.
Styling: Customize the CSS in index.html to adjust the appearance of the map, toolbar, or navigation controls.


Contributing 🤝
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Commit your changes (git commit -m 'Add your feature').
Push to the branch (git push origin feature/your-feature).
Open a Pull Request.

Report issues or suggest enhancements via the Issues tab. 🐛

License 📜
This project is licensed under the MIT License. See the LICENSE file for details.

Español 🇪🇸
VisorVB 🌍
  
VisorVB es un visor de mapas web multipropósito construido con Leaflet, diseñado para integrar múltiples servicios WMS (como el PNOA del IGN de España) con transparencias y opacidades personalizables. Ofrece una interfaz interactiva con una barra de herramientas personalizable, controles de navegación circulares, visualización de coordenadas activable y soporte para superposiciones GeoJSON. Es ideal para visualización geoespacial. 🗺️

📋 Tabla de Contenidos

Características
Instalación
Uso
Personalización
Contribución
Licencia


Características 🚀

Soporte Multi-WMS: Integra múltiples servicios WMS (ej., PNOA) con transparencia y opacidad ajustables para visualización en capas. 🛰️
Navegación Interactiva: Panel circular (inferior derecha) para desplazamiento y centrado del mapa. 🎮
Coordenadas Dinámicas: Muestra coordenadas y nivel de zoom al presionar la tecla 'C' (inferior izquierda). 📍
Barra de Herramientas Personalizable: Barra desplegable (superior izquierda) para añadir herramientas personalizadas. 🛠️
Integración GeoJSON: Superpón datos de parcelas u otras capas geoespaciales mediante GeoJSON. 📊
Diseño Responsivo: Se adapta al 100% del ancho del contenedor padre. 📱💻


Instalación 🔧

Clonar el Repositorio:
git clone https://github.com/RubenBarrionuevo/VisorVB.git


Abrir el Proyecto:

Abre index.html en un navegador moderno (Chrome, Firefox, etc.) sin necesidad de servidor.
Opcionalmente, sirve el proyecto localmente (ej., con Python):python -m http.server 8000

Luego accede a http://localhost:8000.


Dependencias:

Usa Leaflet (v1.9.4) y Font Awesome (v6.0.0) alojados en CDN. No requiere instalación adicional. 🌐




Uso 🖱️

Abrir el Mapa:

Se inicializa centrado en Punta Chullera, Manilva (coordenadas: 36.3217, -5.2489, zoom 17).


Navegación:

Usa el panel circular (inferior derecha) para desplazarte (arriba, abajo, izquierda, derecha) o centrar el mapa. 🧭
Arrastra el mapa o usa la rueda del ratón para hacer zoom.


Visualización de Coordenadas:

Presiona la tecla 'C' para mostrar u ocultar las coordenadas y el nivel de zoom (inferior izquierda). 📍


Barra de Herramientas:

Haz clic en el ícono de herramientas (superior izquierda) para abrir la barra personalizable, que incluye un botón de prueba. 🛠️


Añadir Capas WMS:

Modifica las llamadas a L.tileLayer.wms en index.html para agregar servicios WMS adicionales. Ajusta opacity (0.0 a 1.0) y transparent: true para superposición. 🛰️
Ejemplo: L.tileLayer.wms('WMS_URL', { layers: 'LAYER_NAME', format: 'image/png', transparent: true, opacity: 0.5 }).


Añadir GeoJSON:

Actualiza la variable parcelsGeoJSON o carga un archivo .geojson para superponer datos personalizados. 📊




Personalización 🎨

Capas WMS: Añade múltiples servicios WMS mediante nuevas instancias de L.tileLayer.wms en el código JavaScript. Usa opacity y transparent: true para controlar la visibilidad.
Capas GeoJSON: Modifica parcelsGeoJSON en index.html o usa el código fetch comentado para cargar archivos GeoJSON externos.
Opciones de la Barra de Herramientas: Añade nuevos botones al panel L.Control.Tools en el código JavaScript.
Estilos: Personaliza el CSS en index.html para ajustar la apariencia del mapa, barra de herramientas o controles de navegación.


Contribución 🤝
¡Las contribuciones son bienvenidas! Sigue estos pasos:

Haz un fork del repositorio.
Crea una nueva rama (git checkout -b feature/tu-funcionalidad).
Realiza tus cambios (git commit -m 'Añadir tu funcionalidad').
Envía la rama (git push origin feature/tu-funcionalidad).
Abre un Pull Request.

Reporta problemas o sugiere mejoras en la pestaña Issues. 🐛

Licencia 📜
Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.
