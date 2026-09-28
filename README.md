Ejemplo 1 (Aplicación Web)
Nombre del proyecto: Figuras geométricas - Área y perímetro- PHP.
Descripción del proyecto: Se presenta una pantalla principal con las figuras geométricas más comunes Cuadrado, Circulo y Triangulo, al dar click en las figuras, se da paso a otra pantalla donde se solicita que el usuario capture la medida del lado (para el cuadrado), el radio (para el circulo) y el lado, la base y altura (para el triángulo). Al dar click en el botón de calcular se muestra el resultado del cálculo de área y perímetro de la figura seleccionada.
Tecnologías usadas: HTML5, CSS3, PHP7 e imágenes PNG.
Características principales: En la pantalla principal (archivo index.html) se implementa un pase de variable por URL (método GET) para indicar al formulario de cálculo (archivo operación.php) la figura que el usuario selecciono. En el formulario de cálculo se recibe el dato del método GET y en base a eso de forma dinámica se construye el formulario con los Input’s (Cajas de texto numéricas) según lo necesario para realizar los cálculos, en un proceso posterior pero incluido en el mismo archivo, sereciben los datos capturados por el usuario en los input’s por método POST, además de los input’s de las “medidas” se incluye un formulario hidden “Oculto” que almacena el identificador de la figura y en base a este dato, se manda llamar la función parametrizada de la figura correspondiente que es la encargada de realizar los cálculos y muestra en pantalla los resultados.
Instalación: Opción A – Local: Se requiere un servicio web instalado previamente se recomienda XAMPP o WAMPServer.
Colocar la carpeta de este proyecto en la carpeta de salida del servidor web local que tenga instalado:
En XAMPP la ruta es: c:/xamp/htdocs
En WAMPServer la ruta es: c:/wamp64/www
Opción B – En un servidor Hosting: Se requiere contar con un servidor previamente instalado o rentado y contar con los datos de acceso, ya sea por FTP o CPANEL.
Coloca la carpeta de este proyecto en la carpeta de salida del servidor Histing normalmente estas carpetas pueden estar nombradas de las siguientes formas:
public_html
www
public
Nota importante: verifica que el servidor Hosting soporte PHP7 o superior.
Uso: Opción A – Local: Ejecuta el servicio web previamente instado (XAMPP o WAMPServer) y en un navegar escribe http://localhost/NombreDeLaCarpetaDelProyecto
Nota importante: Si se realizo alguna configuración de puertos se deben de especificar en la dirección. Por ejemplo, si se configuró el puerto 8080 http://localhost:8080/NombreDeLaCarpetaDelProyecto
Opción B: - En un servidor Hosting: En un navegador web accede a la dirección de dominio donde se encuentra la implementación de la página. Por ejemplo, https://www.miDominio.com/figurasGeometricas

Contribuciones: 
¡Las contribuciones son bienvenidas! Si deseas ayudar a mejorar este proyecto, por favor sigue los siguientes pasos:
1.	Haz un fork del repositorio: Crea una copia del repositorio en tu cuenta de GitHub.
2.	Clona el repositorio: Clona tu fork a tu máquina local.
Bash
git clone https://github.com/rodokizzzdev/AyPFigurasPHP.git
3.	Crea una nueva rama: Trabaja en una rama separada para tus cambios.
Bash
git checkout -b nombre-de-tu-rama
4.	Haz tus cambios y commit: Realiza las modificaciones que consideres necesarias y describe claramente tus cambios.
Bash
git add .
git commit -m "Descripción clara de tus cambios"
5.	Envía los cambios a tu repositorio: Sube tus cambios a tu fork en GitHub.
Bash
git push origin nombre-de-tu-rama
6.	Abre un pull request: Desde tu repositorio en GitHub, abre un pull request hacia la rama main del repositorio original. Explica tus cambios y por qué crees que deberían ser integrados.
Una vez que envíes tu pull request, lo revisaré lo antes posible. ¡Gracias por tu interés en mejorar este proyecto!

Licencia: MIT
# Figuras-Geometricas-PHP
Este proyecto permite calcular el ára y perimetro de figuras geometricas basicas
