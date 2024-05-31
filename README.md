REVISTA COSAS Versión 1.1

Este código contienen todos los archivos del sitio web COSAS, los cuales son a nivel frontend y con requerimientos no funcionales. La idea de este sitio es transformar el portal y brindarle al usuario una experiencia intuitiva y amigable, donde se pueda sentir cómodo cuando lea el contenido y navegue enntre las notas.



----------------------------------------------------------------
----------------------------------------------------------------
REGISTRO DE VERSIONES:

1.0 - 17 de mayo del 2024
1.1 - 28 de mayo del 2024



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



----------------------------------------------------------------
----------------------------------------------------------------
404.html

El archivo 404.html que se encuentra dentro de la carpeta "files" es el archivo que debe mostrarse por defecto cuando un página no exita (si es necesario moverlo de ruta puedes hacerlo). Es importante aclarar que no creé ningún archivo htaccess, por lo tanto deberás crear uno para configurar el archivo 404.html como página de defecto.










----------------------------------------------------------------

Actualizaciones 28 de mayo del 2024 (versión 1.1) | INICIO

----------------------------------------------------------------

El 28 de mayo del 2024 agregué dos imágenes a la carpeta "images" cuyos nombre son "cosas404.png" y "cosas4042.png" las cuales aparecen en la página 404.html. Además, agregué el propio archivo 404.html a la carpeta "files". Por último, agregué clases al CSS para configurar el archivo 404.html. Podrás encontrar estas clases en las siguientes líneas:

° Línea 1520 (.contenedor_404{})
° Línea 1529 (.contenedor_404_seccion_1{})
° Línea 1539 (.contenedor_404_seccion_2{})
° Línea 1550 (.contenedor_404_seccion_3{})
° Línea 1560 (.imagen_cosas404{})
° Línea 1579 (.boton_404:hover{})
° Línea 1583 (.boton_404:active{})

Las clases que mencioné preteritamente fueron las que se agregaron al CSS, ahora te meciono las que ya existían y fueron actualizadas:

° Línea 712 (.tarjeta_nota_universal{})
° Línea 963 (.texto_tarjeta_nota_2{})

----------------------------------------------------------------

... | FINAL

----------------------------------------------------------------





----------------------------------------------------------------

Actualizaciones 29 de mayo del 2024 (versión 1.2) | INICIO

----------------------------------------------------------------

El 29 de mayo del 2024 agregué clases al CSS y el JS (main_nota.js), las cuales solucionan el problema que presentaba la página que le corresponde a cada artículo/nota, donde los textos que se generan dentro del contenedor "contenedor_textos_nota" no se les podía aplicar las clases debido a incompatiblidad con wordpress. En las siguientes líneas podrás encontrar las clases que agregué al CSS (no actualicé ninguna otra clase, solo agregué):

° De la línea 3847 a la 3905 (.texto_nota_h1{}, .texto_nota_h2{}, texto_nota_h3{}, .texto_nota_h4{}, .texto_nota_h5{} y .texto_nota_h6{})
° De la línea 3198 a la 3256 (.texto_nota_h1{}, .texto_nota_h2{}, texto_nota_h3{}, .texto_nota_h4{}, .texto_nota_h5{} y .texto_nota_h6{})
° De la línea 391 a la 449 (.texto_nota_h1{}, .texto_nota_h2{}, texto_nota_h3{}, .texto_nota_h4{}, .texto_nota_h5{} y .texto_nota_h6{})


JS:
Con respecto al JS "main_nota.js" agregué más código (el resto de su contenido quedó intacto), el cual le agrega clases a los párrafos, h1, h2, h3, h4, h5 y h6 que se generen dinámicamente a través de Wordpress. Te comparto de que línea a que línea está el contenido nuevo:

° De la línea 290 a la 311

----------------------------------------------------------------

... | FINAL

----------------------------------------------------------------





----------------------------------------------------------------

Actualizaciones 30 de mayo del 2024 (versión 1.3) | INICIO

----------------------------------------------------------------

El 30 de mayo del 2024 agregué y actualicé el nuevo carrusel del index, para agregarlo y actualizarlo solo deberás centrarte en el archivo index.html. Te comparto de que a que líneas están las actualizaciones:

° De la línea 353 a la 389 (section del carrusel que debe actualizarse)

Ahora te comparto de que a que línea está el contenido que debes agregar:

° De la línea 804 a la 896

----------------------------------------------------------------

... | FINAL

----------------------------------------------------------------





----------------------------------------------------------------

Actualizaciones 31 de mayo del 2024 (versión 1.4) | INICIO

----------------------------------------------------------------

El 31 de mayo del 2024 agregué y actualicé el CSS para mejorar la estructura del HTML que le corresponde a cada nota, debido a problemas presentados con wordpress html. Esta actualización agrega clases y modifica otras ya existentes, como primer paso inidcaré cuales fueron agregadas:

° Las líneas: 1581, 1796, 1941, 2234, 2674, 3283, 3997 y 4675 cuentan con clases que fueron agregadas (estado_flex).
° Las líneas: 740, 1672, 1817, 1960, 2249, 2694, 2747, 3334 y 4017 cuentan con clases que fueron agregadas (contenedor_universal_2).



Ahora las clases que fueron actualizadas:

° Las líneas: 1363, 2240, 3434 y 4098 (cotenedor_opciones_nota) 
° Las líneas: 751, 1690, 1828, 2023, 2491, 3072, 3815 y 4498 (contenedor_universal_nota) 
° Las líneas: 1083, 2655, 2758, 3422 y 4086 (contenedor_textos_nota) 



Es muy y sumamente muy importante aclarar debido a que fueron agregadas nuevas clases muy probablemente en el CSS que tengan no se encuentren las clases que fueron actualizadas en las líenas que mencioné, por lo tanto hago una
aclaración por si se desea buscar la clase dentro del css. La primera vez que se menciona la clase (fuera de los media screen) se le aplican estas propiedades:
.cotenedor_opciones_nota{
    display: flex;
    flex-wrap: wrap;
    justify-content: end;
    align-content: center;
    width: 100%;
    height: auto;
    margin-bottom: 25px;
    padding: 20px 0px;
    gap: 10px;
}

.contenedor_universal_nota{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-content: start;
    width: 60%;
    height: auto;
    border-bottom: 2px #eeeeee solid;
    grid-gap: 0px 0px;
}

.contenedor_textos_nota{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-content: start;
    width: 100%;
    height: auto;
}

Las otras veces que se re repite la clase es dentro de los media screen y absolutamente en todos los demás se les aplica las mismas propiedades (esta lógica aplica para las tres clases):
.cotenedor_opciones_nota{
    width: 100%;
    height: auto;
    margin-bottom: 0px;
    padding: 20px 0px;
    gap: 10px;
}

.contenedor_universal_nota{
    width: 100%;
    height: auto;
    border-bottom: 2px #eeeeee solid;
}

.contenedor_textos_nota{
    justify-content: center;
    align-content: start;
    width: 100%;
    height: auto;
}



----------------------------------------------------------------

... | FINAL

----------------------------------------------------------------
