# Repositorio con preguntas de programacion en Python
## ¿A quien va dirijo?
Este quiz asume que el estudiante tiene unos conocimientos basicos de programacion de aplicaciones en ambientes de red usando los protocolos TCP y UDP
## Preliminares
**Antes de comenzar a hacer el quiz debe hacer lo que se describe a continuacion**

Usted debera entrar al siguiente <a href="https://goo.gl/forms/Mqjq9ryqDX4KNt4u1" target="_blank">formulario</a> y digitar alli su **codigo de estudiante** y el **numero IP de la maquina** desde donde esta corriendo el quiz. Para ver como obtener el IP de su maquina por favor visitar este [video](https://asciinema.org/a/0mv94mnarx6wqljoq3yvxklxy).

Una vez hecho esto y haber diligenciado las tres primeras preguntas del formulario correspondientes a codigo de estudiante, nombre e IP; ahora si proseguir con las siguientes preguntas.

## Preguntas
### Pregunta 1
Dado el siguiente codigo, escriba un programa que envie la palabra "HolA"

~~~~
#!/usr/bin/env python
from socket import *
# Llene las siguientes lineas de modo que s sea un socket del tipo TCP
s = socket( , )
# Se debe conectar a la maquina con IP 172.17.9.51 y puerto 9001
s.connect( )
# Se envia la cadena "HolA"
s.send("HolA")
# Complete el codigo que permita recibir los datos en la variable 'data'
data = s.
# Se imprime lo recibido por el servidor
print data
# Cierra el socket
s.close()
~~~~

### Pregunta 2
Dado el siguiente codigo, escriba una aplicacion como se describe en el siguiente codigo

~~~~
#!/usr/bin/env python
from socket import *
# 1- Cree una conexion TCP al servidor cuyo IP es 172.17.9.51 y puerto 9002
# 2- Usted abrira una conexion y recibira dos cadenas de caracteres, en mensajes
#    separados (es decir dos llamados a la funcion socket.recv()). 
#    Cada cadena representa un numero entero. Es seguro que el tamano a recibir #    sea maximo 10 caracteres
# 3- Su programa debe convertir esas cadenas a numeros enteros, hacer una 
#    multiplicacion entre estos numeros y enviar al servidor ese resultado
# 4- Su programa debe recibir una cadena (esta cadena no ocupara mas de 10 bytes
#    de parte del servidor).
#    Su programa debe imprimir la cadena enviada por el servidor
~~~~

Es importante tener en cuenta que en lo que hemos visto de clase, cliente y servidor intercambian cadenas de caracteres pero es posible que estas representen un valor entero. En este [video](https://asciinema.org/a/2hqm3rvjuk048tmbw6qcv8358) se muestran algunas funciones en Python que permiten moverse de entero a cadena y de cadena a entero.


### Pregunta 3

Dado el siguiente codigo, escriba una aplicacion cliente en UDP que imprima una cadena enviada por el servidor
~~~~
#!/usr/bin/env python
from socket import *
# Complete la instruccion en Python de modo que se cree un socket del tipo UDP
s = socket( , )
msg = "HolA"
# Ahora usted enviara el contenido de la variable msg al servidor UDP.
# Entonces, modifique la siguiente linea de modo que 
# - La palabra 'funcion' sea reemplazada por el nombre de la funcion en Python
#   que envia datos a traves de un socket UDP
# - El segundo argumento de la funcion de envio de los datos sean los datos
#   correspondientes al servidor cuyo IP es 172.17.9.51 numero de puerto 9001
s.funcion( , )
# Ahora reciba los datos del servidor. Cambie la palabra 'funcion1' por el 
# nombre de la funcion que se usa para recibir datos a traves de un socket UDP
data, addr = s.funcion1(100)

print "%s"%(data)
~~~~
 
