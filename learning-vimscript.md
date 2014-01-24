###\#0

####Prerequisitos

Versión actual estable: 7.4. Este lenguaje no es específico para Vim en consola, GUI Vims (gVim o MacVim). Veremos terminología como `buffer`, `window`, `normal mode`, `insert mode` y `text object`.

####Creando un fichero .vimrc

El fichero `~/.vimrc` contiene código escrito en Vimscript. Vim ejecutará este código cada vez que arranque. En linux y mac el fichero es `.vimrc`. En windows el fichero se llama `_vimrc`.

Para saber cual es la ruta de este fichero en nuestro sistema podemos consultarlo estando dentro de Vim con el siguiente comando:  `:echo $MYVIMRC`. 

###\#1 

####Mostrando mensajes

Empezamos con los comandos `echo` y `echom`. Dentro de Vim, siempre y cuando tengas instalada la documentación, se puede consultar la ayuda de cualquier comando ejecutando: `:help echo` o `:help echom`. 

Prueba de ejecutar: `:echo "Hello world"` y te Vim te mostrará el texto en la línea inferior que es la línea de información en la que podemos consultar información del texto que estamos editando y ver los mensajes de información que nos da Vim. 

####Mostrando mensajes de forma persistente

Para que nuestro mensaje se quede en el `log` de Vim, al cual podemos acceder ejecutando el comando `:messages`, tenemos que utilizar el comando `echom` en lugar de sólamente `echo`. 

####Comantarios

Los comentarios en Vimscript se ponen con las comillas dobles.

###\#2

####Configurando las opciones

Hay dos principales tipos de opciones: las lógicas y las opciones que reciben un valor. 

#####Opciones lógicas

Son como un interruptor, por ejemplo para activar la opción de que se muestre el número de línea, podemos ejecutar: `:set number` o para quitarlas podemos ejecutar `:set nonumber`. 

Por tanto, todas las opciones lógicas (*boolean*) funcionan con este patrón: `:set <name>` y para apagarlas usaremos el patrón: `:set no<name>`.

También podemos *toglear* las opciones lógicas de forma que hacemos que valgan lo opuesto a lo que valen. Esto sirve para activar y desactivar rápidamente una opción, para ello podemos ejecutar el comando: `:set number!`.

Para comprobar el estado de una variable lógica pondremos al final un signo de interrogación (bastante lógico y normal ¿no? esto es así porque en Vim los comandos serán muy parecidos a como si hablásemos con el ordenador). Por tanto para conocer el estado de la opción `name` haremos: `:set number?`.

#####Opciones que reciben valores

Algunas opciones reciben valores en lugar de activarse o desactivarse, el patrón para asignar valores es: `:set <variable>=<valor>`. Y para comprobar su valor lo haremos de igual forma que con las variables lógicas, usando un signo de interrogación. Por último, es interesante saber que se pueden ejecutar y asignar diferentes variables en un mismo comando, por ejemplo activar la oción de número de líneas y asignar un valor a una variable: `:set number numberwidth=6`.

WIP
Next: http://learnvimscriptthehardway.stevelosh.com/chapters/03.html





###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
###\#1
