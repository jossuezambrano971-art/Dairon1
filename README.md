def calcular_promedio(numeros):
    suma = 0
    contador = 0
    resultado = 0  # Variable innecesaria

    for n in numeros:
        suma = suma + n
        contador = contador + 1

    promedio = suma / contador  # Posible división por cero
    return promedio


def imprimir_resultado():
    datos = []  # Lista vacía (error lógico)
    promedio = calcular_promedio(datos)
    print("El promedio es: " + promedio)  # Error de tipo (str + float)


def funcion_insegura():
    password = "123456"  # Credencial hardcodeada (problema de seguridad)
    print("La contraseña es:", password)


def codigo_mal_estilo():
    x=10
    y=5
    if x>y:
     print("x es mayor que y")  # Mala indentación


def main():
    imprimir_resultado()
    funcion_insegura()
    codigo_mal_estilo()
    variable_no_usada = 100  # Variable declarada y no utilizada


main()

