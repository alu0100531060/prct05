#!usr/bin/python
#!encoding: UTF-8

import sys

# def calcular_xi (n, i):
#xi = (i -1.0/2.0) / n               # Esta es una función que podemos emplear.
#return xi

argumentos = sys.argv[1:]
print argumentos                     # Nos visualiza por pantalla una lista con los parámetros que nosotros introduzcamos.

if (len(argumentos) == 1):           #Si la lista tiene un elemento se ejecuta el if, en caso contrario te lo pide por pantalla.
    n = int (argumentos[0])
else:
    print"Introduzca el nº de intervalos (n>0): "
    n = int (raw_imput())
    
if (n>0):
    PI35 = 3.1415926535897931159979634685441852    #Muestra el valor real de la constante pi.
    sumatorio = 0.0
    ini = 0
    intervalos = 1.0 / float (n)
    for i in range (n):
       x_i = ((i+1) - 1.0/2.0) / n  # Aquí se puede utilizar la funcion def que hemos puesto antes.
       fx_i = 4.0 / (1+x_i * x_i)
       print "Subintervalo: [", ini, ",", ini+intervalos, "] x_i:", x_i,"fx_i:", fx_i
       ini += intervalos
       sumatorio += fx_i
    valor_pi = sumatorio / n
    print "El valor de la aproximación de PI es:", valor_pi
    print "El valor de Pi con 35 decimales es: %10.35f" % PI35
else:
    print "El valor de los intervalos debe ser positivo" # El valor de los subintervalos nunca puede ser negativo.