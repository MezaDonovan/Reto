# Reto Codigo Becario

def sumarNumeros(a,b): # Definimos la función sumarNumeros con dos parámetros a y b
  if isinstance(a, int) and isinstance(b, int): # Verificamos si ambos valores son enteros
    resultado = a + b # Realizamos la suma de los dos valores
    return f"El resultado de la suma es: {resultado} SW" # Devolvemos el resultado en formato de cadena de texto
  else: # Si alguno de los valores no es un entero, devolvemos un mensaje de error
      return "Error: Ambos valores deben ser enteros" #  Mensaje que se mostrara en caso de error

# Pruebas de Funcionamiento
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
