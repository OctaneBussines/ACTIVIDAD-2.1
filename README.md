# ACTIVIDAD-2.1
Informe de Instalación y Creación de Proyecto Ionic con Plantilla Tabs
1. Introducción
Este documento describe el procedimiento para la instalación del entorno de desarrollo Ionic, así como la creación y ejecución de un primer proyecto utilizando la plantilla predeterminada Tabs.
Ionic es un framework para el desarrollo de aplicaciones móviles híbridas que utiliza tecnologías web (HTML, CSS y JavaScript) y permite compilar para Android, iOS y web.

2. Requisitos Previos
Antes de iniciar la instalación, es necesario contar con:

Node.js (versión LTS recomendada).

NPM (se instala junto con Node.js).

Conexión a Internet.

Editor de código (Visual Studio Code recomendado).

3. Instalación del Entorno
3.1 Instalación de Node.js
Descargar Node.js desde https://nodejs.org, seleccionando la versión LTS.

Instalar con las opciones predeterminadas.

Verificar la instalación ejecutando en la terminal:

bash
Copiar
Editar
node -v
npm -v
3.2 Instalación de Ionic CLI
Abrir una terminal (CMD, PowerShell o bash).

Ejecutar:

bash
Copiar
Editar
npm install -g @ionic/cli
Confirmar que se instaló correctamente:

bash
Copiar
Editar
ionic -v
4. Creación del Primer Proyecto Tabs
4.1 Generar el Proyecto
En la carpeta de trabajo, ejecutar:

bash
Copiar
Editar
ionic start miPrimerTabs tabs
miPrimerTabs: nombre del proyecto.

tabs: plantilla predeterminada con navegación por pestañas.

Seleccionar el framework deseado (Angular recomendado).

Aceptar integración con Capacitor para compilaciones móviles.

4.2 Ingresar al Proyecto
bash
Copiar
Editar
cd miPrimerTabs
4.3 Ejecutar en el Navegador
bash
Copiar
Editar
ionic serve
La aplicación se abrirá en el navegador mostrando las pestañas Tab 1, Tab 2 y Tab 3.

5. Ejecución en Dispositivos (Opcional)
5.1 Android
bash
Copiar
Editar
ionic capacitor add android
ionic capacitor run android
5.2 iOS (requiere macOS y Xcode)
bash
Copiar
Editar
ionic capacitor add ios
ionic capacitor run ios
6. Estructura de Proyecto
Dentro de src/app/pages/ se encuentran:

tab1/ → Contenido de la pestaña 1.

tab2/ → Contenido de la pestaña 2.

tab3/ → Contenido de la pestaña 3.

Cada carpeta contiene:

HTML → Vista.

TS → Lógica.

CSS/SCSS → Estilos.

7. Problemas Comunes
Comando “ionic” no reconocido: verificar que npm global esté en el PATH del sistema.

Restricciones en PowerShell: ejecutar:

powershell
Copiar
Editar
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
Permisos en macOS/Linux: usar nvm o configurar un prefijo global en npm.
