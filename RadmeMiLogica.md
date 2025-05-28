# Reto Codigo Becario

En este reto debemos realizar una funcion la cual debe identificar entre dos numeros que ambos sean enteros y realizar el procedimiento de suma, en caso contrario de tener un algun número no entero o algun otro caracter que no sea un número debera mostrar un error de funcionamiento exigiendo que ambos sean numeros enteros.

-Primero se debe definir la funcion que utilizaremos para la suma, en este caso "sumarNumeros" será nuestra funcion.
-Posteriormente Debemos Verificar que ambos parametros que recibe la funcion son valores enteros, esto con ayuda de la funcion isinstance que nos ayuda a clasificar si el objeto recibido es un numero entero o no lo es.
-Al verificar que nuestros valores recibidos son enteros pasamos a la suma de ambos y guardamos el resultado en la variable "resultado"
-En caso contrario, si alguno o ambos de los valores no son de tipo entero retornara un mensaje de error, pidiendo que ambos valores sean enteros.
def sumarNumeros(a,b): # Definimos la función sumarNumeros con dos parámetros a y b
  if isinstance(a, int) and isinstance(b, int): # Verificamos si ambos valores son enteros
    resultado = a + b # Realizamos la suma de los dos valores
    return f"El resultado de la suma es: {resultado} SW" # Devolvemos el resultado en formato de cadena de texto
  else: # Si alguno de los valores no es un entero, devolvemos un mensaje de error
      return "Error: Ambos valores deben ser enteros" #  Mensaje que se mostrara en caso de error
#Pruebas de Funcionamiento
print(sumarNumeros(5,3))
print(sumarNumeros(-10,4))
print(sumarNumeros(0,0))
print(sumarNumeros(123,877))
print(sumarNumeros(2,5.5))
print(sumarNumeros("10",5))
print(sumarNumeros(8,None))
print(sumarNumeros("True",3))
print(sumarNumeros([ ],{}))
print(sumarNumeros(5,85))
print(sumarNumeros(-1000,445))
print(sumarNumeros(885,.5563))
print(sumarNumeros(5,"s"))
print(sumarNumeros(5.8,"a"))
print(sumarNumeros("a","b"))
