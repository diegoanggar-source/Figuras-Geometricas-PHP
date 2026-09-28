# Figuras-Geometricas-PHP

Este proyecto permite calcular el **área y perímetro de figuras geométricas básicas** mediante una aplicación web desarrollada con PHP.

## 📋 Descripción del proyecto

La aplicación presenta una pantalla principal con algunas de las figuras geométricas más comunes:

* Cuadrado
* Círculo
* Triángulo

Al seleccionar una figura, el usuario es dirigido a otra pantalla donde debe ingresar las medidas necesarias para realizar el cálculo.

Dependiendo de la figura seleccionada, se solicitan diferentes datos:

* **Cuadrado:** lado.
* **Círculo:** radio.
* **Triángulo:** lado, base y altura.

Al presionar el botón **Calcular**, la aplicación realiza las operaciones correspondientes y muestra en pantalla el **área y perímetro** de la figura seleccionada.

## 🛠️ Tecnologías utilizadas

* **HTML5** – Estructura de las páginas web.
* **CSS3** – Diseño y estilos de la aplicación.
* **PHP 7** – Procesamiento de datos y cálculos.
* **Imágenes PNG** – Representación visual de las figuras geométricas.

## ⭐ Características principales

La aplicación cuenta con las siguientes características:

1. **Pantalla principal**

   * Muestra las figuras geométricas disponibles.
   * Permite seleccionar una figura para realizar sus cálculos.

2. **Envío de información mediante GET**

   * Desde el archivo `index.html` se utiliza el método **GET** para enviar mediante la URL el identificador de la figura seleccionada.
   * Esto permite que el archivo `operacion.php` conozca qué figura debe procesar.

3. **Formulario dinámico**

   * El archivo `operacion.php` recibe el dato enviado mediante GET.
   * Dependiendo de la figura seleccionada, construye dinámicamente el formulario con los campos necesarios.
   * Por ejemplo:

     * Para el cuadrado se solicita el lado.
     * Para el círculo se solicita el radio.
     * Para el triángulo se solicitan el lado, la base y la altura.

4. **Envío de datos mediante POST**

   * Una vez que el usuario captura las medidas, los datos son enviados mediante el método **POST**.
   * Además de las medidas, se utiliza un campo `hidden` para conservar el identificador de la figura seleccionada.

5. **Cálculo de área y perímetro**

   * De acuerdo con el identificador de la figura, se llama a la función correspondiente.
