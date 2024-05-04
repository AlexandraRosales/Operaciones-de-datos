# Operaciones-de-datos
Código:
#Declaramos la función encontar_cuadrante con los argumentos (x,y) que son nuestras variables.
def  encontrar_cuadrante(x, y):
    #Declaramos la primera condición (x,y) aceptan todos los valores mayores a cero.
    if x > 0 and y > 0:
        #Si cumple la condición, imprime la "I" (uno) que corresponde  donde se encuentra el punto. 
        return "I"
    #La segunda condición verifica si "x" es menor a 0 y "y" mayor a cero.
    elif x < 0 and y > 0:
        #De ser así, imprime "II" (dos) que corresponde a donde se encuentra el punto.
        return "II"
        #la tercera condición verifica si ambas variables son menores a cero.
    elif x < 0 and y < 0:
        #Al cumplir la condición imprime "III" (tres) que corresponde a donde se encuentra el punto.
        return "III"
        #La cuarta condición verifica si "x" es mayor y "y" menor a cero.
    elif x > 0 and y < 0:
        #Si cumple, imprime "IV" (cuatro) que corresponde a donde se encuentra el punto.
        return "IV"
        #La ultima condición si escriben 0 en "x" y "y".
    else:
        #Imprime el mensaje si ninguna de las condiciones anteriores es verdadera.
        return "en el origen"
 #Definimos una función llamada main.
def main():
    #Imprime para que sirve este programa.
    print("Programa para encontrar el cuadrante mediante las coordenadas ingresadas.")
    #Imprime los cuadrantes existentes con sus signos correspondientes.
    print("X,Y:\n(+,+)=> Cuad. I\n(-,+)=> Cuad. II\n(-,-)=> Cuad. III\n(+,-)=> Cuad. IV")
    #Declaramos las variables x,y de tipo float para que el usuario pueda ingresar las coordenadas solicitadas.
    x = float(input("\nIngrese X: "))
    y = float(input("Ingrese Y: "))
#La condición verifica que ambas variables sean igual a 0.
    if x == 0 or y == 0:
        #Si alguna de las coordenadas es 0, imprime mensaje de error.
        print("¡Ups! Las coordenadas no pueden ser cero, inténtalo más tarde.")
        #Si ninguna de las coordenadas escritas es 0 ejecutará las siguientes líneas del código.
    else:
        #Llamamos a la función encontrar_cuadrante con las coordenadas (x,y) que se guaradará en la variable cuadrante.
        cuadrante = encontrar_cuadrante(x, y)
        #Imprime el mensaje mostrado en que cuadrante se encuentra el punto, utilizando f-strings para incluir el valor de la variable cuadrante.
        print(f"El punto se encuentra en el cuadrante {cuadrante}.")
        
#Esta línea comprueba si el script se ejecuta correctamente
if __name__ == "__main__":
    #Llama a la función main para iniciar la ejecución del programa.
    main()

    Reflexión: El bootcamp ha sido de mucha ayuda y aprendizaje para la resolución de problemas lógicos y un tanto matemáticos mostrando las posibilidades y lo útil que es la condicional if else en los programas. Hasta el momento Python es un lenguaje muy interesante y con una sintaxis muy simple.
