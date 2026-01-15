def funcion_compleja(a, b, c):
    if a > 0:
        if b > 0:
            if c > 0:
                print("Todos son positivos")
            else:
                print("c no es positivo")
        else:
            print("b no es positivo")
    else:
        print("a no es positivo")


def funcion_compleja_duplicada(a, b, c):
    if a > 0:
        if b > 0:
            if c > 0:
                print("Todos son positivos")
            else:
                print("c no es positivo")
        else:
            print("b no es positivo")
    else:
        print("a no es positivo")


def funcion_con_asuntos():
    password = "123456" 

    x = 10
    y = 0
    resultado = 0  

    if y != 0:
        resultado = x / y
    else:
        print("División por cero evitada")


def funcion_no_usada():
    print("Nunca se ejecuta")


def main():
    funcion_compleja(1, 2, 3)
    funcion_compleja_duplicada(1, 2, 3)

    variable_sin_uso = 100 

    if True == True:       
        print("Condición innecesaria")


main()




