# Imagemagic en WAMP con PHP7.1

- [x] aledc.com

## Este documento describe el procedimiento para hacer funcionar el módulo de php ImageMagic  en Windows con WAMPP Y PHP 7.1

Esta solución funcioará en Windows de 64 Bits, con la opción de Thread Enable.

1 - descargar los archivos **"ImageMagick-6.9.3-7-vc14-x64"**   y **"php_imagick-3.4.3-7.1-ts-vc14-x64"** incluídos en este repo.

2 - descomprimir "php_imagick-3.4.3-7.1-ts-vc14-x64" y copiar todo el contenido en la ruta:
```
"C:\wamp64\bin\php\php7.1.22\ext\"
```
3 - descomprimir "ImageMagick-6.9.3-7-vc14-x64" y copiar tpodos los archivos que empiezan con CORE_RL o con IM_MOD en la siguiente ruta: 
```
C:\wamp64\bin\php\php7.1.22\
````
4 - Agregar al php.ini la siguiente linea:
```
extension=php_imagick.dll
```
5 - Reiniciar el server Wamp

6 - Verificar en el phpinfo()  buscando el texto "imagick" deberia aparecer como módulo.


Eso es todo.


NOTA:  en caso de que tengas otra version de PHP distinta a la 7.1, o que tengas Thread discable, en este enlace podrás encontrat todas las versiones disponibles.

https://mlocati.github.io/articles/php-windows-imagick.html

