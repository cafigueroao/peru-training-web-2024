---
layout: page
title: WEAP - Esquemática
parent: Martes 2 de julio
nav_order: 1
---

# ESQUEMÁTICA
La Vista Esquemática sirve como punto de partida para todas las actividades en WEAP. A continuación, se presentan los elementos que la componen junto con las funcionalidades que cada uno ofrece:

*	Leyenda de WEAP

<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 50%; border: 0px;">
      <img src="../images/01_Dia_1/WEAPElementos/Figura_1.png" alt="Esquema WEAP" style="max-width: 100%;">
    </td>
    <td style="width: 50%; border: 0px;">
      La Vista Esquemática es el punto de partida para todas las actividades en WEAP. Una característica central de WEAP es su interfaz gráfica de "arrastrar y soltar" fácil de usar, que se emplea para describir y visualizar las características físicas del sistema de oferta y demanda de agua. Este diseño espacial se denomina esquema. Puede crearlo, editarlo y visualizarlo en la Vista Esquemática. Se pueden agregar capas SIG para brindar mayor claridad e impacto.
    </td>
  </tr>
</table>

<div style="text-align:center">
    <img src="../images/01_Dia_1/WEAPElementos/Figura_2.gif" alt="Esquema WEAP" width="90%">
</div>
<br>

* Gestor de Capas SIG en WEAP

El gestor de capas SIG en WEAP es una herramienta fundamental para <b>visualizar</b>, datos geográficos dentro del contexto de la herramienta. Su principal función reside en la superposición de información espacial sobre el esquema WEAP, permitiendo al usuario representar gráficamente elementos geográficos como ríos, cuencas hidrográficas, límites políticos, infraestructura hidráulica y otros datos relevantes para el análisis del sistema hídrico. Esto facilita la comprensión espacial del modelo y la identificación de patrones o relaciones entre los componentes del sistema.

Este gestor presenta las siguientes funcionalidades:

<table style="width: 100%; border: 0px; border-collapse: collapse; text-align:justify;">
  <tr>
    <td style="width: 30%; border: 0px;">
      Casilla de verificación <br>
Esta función permite que cada capa se pueda ocultar o mostrar en el esquema. También permite ocultar o mostrar todos los mapas a la vez, haciendo clic derecho en la lista de capas de fondo y seleccionando "Ocultar o Mostrar todas las capas.
</td>
    <td style="width: 70%; border: 0px;">
      <img src="../images/01_Dia_1/WEAPElementos/Figura_3.gif" alt="Esquema WEAP" style="max-width: 100%;">
    </td>
  </tr>
</table>

* test

<a href="#imagen-popup" class="popup-link">
    <img src="../images/01_Dia_1/WEAPElementos/Figura_3.gif" alt="Descripción de la imagen">
</a>

<div id="imagen-popup" class="popup">
    <img src="../images/01_Dia_1/WEAPElementos/Figura_3.gif" alt="Descripción de la imagen">
    <a href="#" class="cerrar-popup">Cerrar</a>
</div>

<style>
    /* Estilos para el pop-up */
    .popup {
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        background: white;
        padding: 20px;
        border: 1px solid #ccc;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
        display: none;
        z-index: 9999;
    }

    .popup img {
        max-width: 100%;
        height: auto;
        display: block;
        margin: 0 auto;
    }

    .popup-link {
        display: block;
    }

    .cerrar-popup {
        display: block;
        text-align: center;
        margin-top: 10px;
        color: #555;
    }
</style>

<script>
    // JavaScript para mostrar y ocultar el pop-up al hacer clic
    document.addEventListener('DOMContentLoaded', function() {
        var popupLink = document.querySelector('.popup-link');
        var popup = document.getElementById('imagen-popup');
        var cerrarPopup = document.querySelector('.cerrar-popup');

        popupLink.addEventListener('click', function(e) {
            e.preventDefault();
            popup.style.display = 'block';
        });

        cerrarPopup.addEventListener('click', function(e) {
            e.preventDefault();
            popup.style.display = 'none';
        });
    });
</script>

