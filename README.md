# ImageMagic en Windows con Wamp y php 7.1
[![aledc.com](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.com)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.com)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.com)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.com)


- [x] aledc.com
- [x] PHP 7

Este Documento describe el procedimiento para hacer funcionar el módulo de php ImageMagic en Windows con Wampp Y php 7.1

ImageMagic es un módulo de PHP qe permite obtener una imágen partiendo de un documento PDF.

Esta solución fue probada en Windows 10 de 64 Bits, con la opción de php Thread Enable.

1 - Descargar los archivos:  

 [ImageMagick-6.9.3-7-vc14-x64](https://drive.google.com/file/d/1nWAXI-DZPObBqGLROsSOHZFYur4SzN47/view?usp=sharing)   
 [php_imagick-3.4.3-7.1-ts-vc14-x64](https://drive.google.com/file/d/1yrjMDFAFr62XalgGfhkDYn-peRaeKtxi/view?usp=sharing)
 
 

2 - Descomprimir "php_imagick-3.4.3-7.1-ts-vc14-x64" y copiar todo el contenido en la ruta:
```
"C:\wamp64\bin\php\php7.1.22\ext\"
```


3 - Descomprimir "ImageMagick-6.9.3-7-vc14-x64" y copiar tpodos los archivos que empiezan con CORE_RL o con IM_MOD en la siguiente ruta: 
```
C:\wamp64\bin\php\php7.1.22\
````


4 - Agregar al php.ini la siguiente linea:
```
extension=php_imagick.dll
```


5 - Reiniciar el server Wamp



6 - Verificar en el phpinfo()  buscando el texto "imagick" deberia aparecer como módulo.


7 - Por último , he subido un archivo imagic.php  que contiene un ejemplo completo de ImageMagic que convertirá archivo 'ale.pdf' a un archivo jpg llamado 'archivo_de_salida.jpg'.    
 Este ejemplo tiene todo el código comentado de manera que puedas adaptarlo a tus necesidades.


Eso es todo.


NOTA:  en caso de que tengas otra version de PHP distinta a la 7.1, o que tengas Thread disable, en este enlace podrás encontrat todas las versiones disponibles.

[ImageMagic Otras Versiones](https://mlocati.github.io/articles/php-windows-imagick.html)

