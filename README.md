REVISTA COSAS Versión 1.0

Este código contienen todos los archivos del sitio web COSAS, los cuales son a nivel frontend y con requerimientos no funcionales. La idea de este sitio es transformar el portal y brindarle al usuario una experiencia intuitiva y amigable, donde se pueda sentir cómodo cuando lea el contenido y navegue enntre las notas.



----------------------------------------------------------------
----------------------------------------------------------------
ARQUITECTURA:

Dentro de la raíz encontrarás un archivo HTML y dos carpetas principales, una de ellas bajo el nombre de "assets" y la otra con con el nombre de "files". Ambas poseen archivos internos y subcarpetas, siendo la carpeta "assets" la encargada de almacenar todo el contenido gráfico y lógico. En cambio, "files", posee el archivo nota.html y resultados.html los cuales, como su nombre lo dice, son encargados de fungir dentro del portal. Ejemplo, nota.html es el archivo que le corresponde a cada nota (las cuales se generan dinámicamente a través de las configuraciones que se hayan hecho en php por parte del frontend) y resultados.html es la interfaz que tendrá la sección de resultados del sitio web, aquella página que aparece por defecto cuando el usuario busca algo a través de la barra de búsqueda.


 
----------------------------------------------------------------
----------------------------------------------------------------
INDEX:

El archivo index está dividido por secciones, las separan cada sección del sitio web. Estas están bajo la clase "contenedor_universal", la cual posee propiedades especiales que le permitirán al contenido de tu sección tener un diseño responsivo, sin embargo asegurate de que el contenido esté bien programado y si posee características distintas a las del resto del código, entonces deberás cerciorarte que la sección sea compatible con tu código especial.



----------------------------------------------------------------
----------------------------------------------------------------
JavaScript (Main):

Aquí podrás encontrar una gran cantidad de código encargada de darle vida a tu sitio web, las cuales tienen como finalidad satisfacer los requerimientos no funcionales y uno que otro funcional. Si deseas controlar y modificar el menú que aparece en los dispositivos móvile (Se le conoce como menú sandwich) en el Js puedes hacerlo, o por lo menos un 50%, ya que el otro 50% también depende del CSS. Regresando al tema, este archivo te permitirá aplicarle una animación al menú, tanto al abrirlo como al cerrarlo, mientras que el css es el responsable y encargado de hacer que el contenido desaparezca o aparezca según las dimensiones (a lo ancho) del dispositivo.



----------------------------------------------------------------
----------------------------------------------------------------
Configuración en pantallas (CSS - Media screen):

Todos los archivos se apoyan del mismo css para controlar como se vería el contenido en diferentes dispositivos, te dejo la lista de todas las configuraciones:

° 1200px a 1400px
° 1100px a 1199px
° 800px a 1099px
° 600px a 799px
° 500px a 599px
° 300px a 499px
° 0px a 299px

El uso de los media screen tiene como finalidad obtener un mayor control del comportamiento del código y que sea más fácil atender el problema sin la necesidad de complicarnos con la clase principal (la que está fuera de los media screen).



----------------------------------------------------------------
----------------------------------------------------------------
Paleta de colores:

La paleta de colores que maneja el sitio web no es algo del otro mundo y por defecto cada clase que necesite llevarla ya la tiene programada en el CSS, sin embargo, si vas a añadir nuevo código, te dejo la paleta de colores implementada tanto en los textos como en los contenedores:

° Color blanco (el fondo y otros elementos que lo apliquen): #ffffff

° Color rojo (texto y la barra de progreso de las notas): #e30613, active: a9000b, hover: e30613 y para cambiar el color de las imágenes al hacer hover: "filter: invert(10%) sepia(100%) saturate(5000%) hue-rotate(0deg);"

° Color del texto : #000000