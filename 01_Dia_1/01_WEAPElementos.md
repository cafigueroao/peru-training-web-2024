---
layout: page
title: WEAP - Esquemática
parent: Martes 2 de julio
nav_order: 1
---

# ESQUEMÁTICA
La Vista Esquemática sirve como punto de partida para todas las actividades en WEAP. A continuación, se presentan los elementos que la componen junto con las funcionalidades que cada uno ofrece:

*	Leyenda de WEAP
<!-- Esquema WEAP (Tabla 1) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 50%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_2.gif" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_1.png" alt="Esquema WEAP" style="max-width: 100%;">
      </a>
    </td>
    <td style="width: 50%; border: 0px;">
      La Vista Esquemática es el punto de partida para todas las actividades en WEAP. Una característica central de WEAP es su interfaz gráfica de "arrastrar y soltar" fácil de usar, que se emplea para describir y visualizar las características físicas del sistema de oferta y demanda de agua. Este diseño espacial se denomina esquema. Puede crearlo, editarlo y visualizarlo en la Vista Esquemática. Se pueden agregar capas SIG para brindar mayor claridad e impacto.
    </td>
  </tr>
</table>
<br>

* Gestor de Capas SIG en WEAP

El gestor de capas SIG en WEAP es una herramienta fundamental para <b>visualizar</b>, datos geográficos dentro del contexto de la herramienta. Su principal función reside en la superposición de información espacial sobre el esquema WEAP, permitiendo al usuario representar gráficamente elementos geográficos como ríos, cuencas hidrográficas, límites políticos, infraestructura hidráulica y otros datos relevantes para el análisis del sistema hídrico. Esto facilita la comprensión espacial del modelo y la identificación de patrones o relaciones entre los componentes del sistema.

Este gestor presenta las siguientes funcionalidades:
<!-- Gestor de Capas SIG en WEAP (Tabla 2) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 60%; border: 0px;">
      <b>Casilla de verificación</b><br>
Esta función permite que cada capa se pueda ocultar o mostrar en el esquema. También permite ocultar o mostrar todos los mapas a la vez, haciendo clic derecho en la lista de capas de fondo y seleccionando "Ocultar o Mostrar todas las capas.
</td>
    <td style="width: 40%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_3.gif" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_4.png" alt="Casilla de verificación" style="max-width: 100%;">
      </a>
    </td>
  </tr>
</table>
<br>

<!-- Gestor de Capas SIG en WEAP (Tabla 3) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 40%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_5.gif" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_5.png" alt="Agregar una capa vectorial o raster" style="max-width: 100%;">
      </a>
    </td>
    <td style="width: 60%; border: 0px;">
      <b>Agregar una capa vectorial o raster</b><br>
      Haga clic derecho en el gestor de capas SIG y seleccione "Agregar capa vectorial" o "Agregar capa ráster" según su interés. 
      Referente a las capas vectoriales, WEAP ofrece mucha flexibilidad para elegir colores de mapa, datos, estilos y etiquetas para la visualización, lo que puede ser muy útil para resaltar varias características de las capas.  También le permite eliminar, establecer etiquetas o reordenar los mapas de fondo.
Tenga en cuenta que puede eliminarlos si lo desea, pero su esquema debe tener al menos una capa de fondo (ya sea una capa precargada o una propia). 
    </td>
  </tr>
</table>

<b>Nota</b>: Todas las capas de fondo deben usar la misma proyección geográfica. Si agrega una capa y no aparece en el Esquema, puede deberse a que no usa la misma proyección que las capas de fondo existentes. Las capas globales precargadas de WEAP utilizan la proyección WGS84. Si desea agregar capas que utilizan una proyección diferente a WGS84, debe hacer lo siguiente (Tenga en cuenta que debe hacer esto ANTES de agregar cualquier objeto WEAP, como ríos o sitios de demanda, porque cuando los agregue, utilizarán la proyección vigente y desaparecerán cuando cambie a una proyección diferente):

1. Agregue una de sus capas.
2. Elimine todas las capas (como las capas precargadas) que estén en una proyección diferente.
3. Vaya a "Establecer límites del área" y configure el límite usando su nueva capa.
4. Si su capa es visible en el Esquema, entonces lo ha hecho correctamente.

<!-- Gestor de Capas SIG en WEAP (Tabla 4) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 60%; border: 0px;">
      <b>Agregar mapas base</b><br>
        Haga clic derecho en el visor geográfico 
        Seleccione la opción “Background Image Layer” y ahí la capa de su preferencia
    </td>
    <td style="width: 40%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_6.gif" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_6.png" alt="Casilla de verificación" style="max-width: 100%;">
      </a>
    </td>
  </tr>
</table>
<br>

*	Vista Esquema Detallado

<!-- Gestor de Capas SIG en WEAP (Tabla 5) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 40%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_7.png" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_7.png" alt="Agregar una capa vectorial o raster" style="max-width: 100%;">
      </a>
    </td>
    <td style="width: 60%; border: 0px;">
      Este pequeño esquema siempre mostrará su área completa brindando la posibilidad de acercar y alejar la visualización en el esquema principal. El área que se muestra actualmente en el esquema principal se indica mediante un cuadro rojo en el esquema detallado. 
Haga clic y arrastre en el esquema detallado para cambiar lo que se muestra en el esquema principal. 
También puede mover la barra de zoom (debajo del esquema detallado) o usar la rueda del mouse para acercar o alejar la imagen (con la tecla ctrl presionada y la rueda del mouse, el zoom será más rápido). 
    </td>
  </tr>
</table>

* Visor geográfico

<!-- Visor geográfico (Tabla 6) -->
<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 60%; border: 0px;">
      El visor geográfico (Main Schematic) es una representación visual interactiva que permite a los usuarios diseñar y gestionar los elementos del modelo y sirve para varias funciones clave como lo son:
a) Creación de Modelos: Permite a los usuarios crear un esquema visual del sistema a analizar, permitiendo incluir elementos como ríos, embalses, áreas de demanda y otras infraestructuras relacionadas con el agua.
b) Edición de Objetos: Los usuarios pueden agregar, mover y editar objetos en el esquema arrastrando y soltando símbolos desde la leyenda de WEAP. También pueden hacer clic derecho en los objetos para acceder a opciones adicionales como editar propiedades generales, datos específicos y ver resultados.
c) Navegación y Manipulación: Incluye herramientas para desplazarse y hacer zoom en el esquema, facilitando la visualización y edición de diferentes partes del modelo. 
d) Acceso Rápido a Análisis: Ofrece acceso directo a las variables de datos y tablas de resultados mediante clic derecho en cualquier elemento del esquema. Esto permite una edición y revisión rápida de los datos y resultados dentro del modelo
    </td>
    <td style="width: 40%; border: 0px;">
      <a href="../images/01_Dia_1/WEAPElementos/Figura_7.gif" target="_blank">
        <img src="../images/01_Dia_1/WEAPElementos/Figura_7.png" alt="Visor geográfico" style="max-width: 100%;">
      </a>
    </td>
  </tr>
</table>
<br>
