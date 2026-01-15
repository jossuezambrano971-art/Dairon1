# Archivo: ejemplo_codacy.py
# Código intencionalmente defectuoso para análisis en Codacy

def validar_usuario(usuario, edad, activo):
    # Complejidad alta (muchos if anidados)
    if usuario is not None:
        if usuario != "":
            if edad > 0:
                if edad < 120:
                    if activo == True:
                        print("Usuario válido y activo")
                    else:
                        print("Usuario válido pero inactivo")
                else:
                    print("Edad inválida")
            else:
                print("Edad inválida")
        else:
            print("Usuario vacío")
    else:
        print("Usuario nulo")


def validar_usuario_duplicado(usuario, edad, activo):
    # Duplicación casi exacta del método anterior
    if usuario is not None:
        if usuario != "":
            if edad > 0:
                if edad < 120:
                    if activo == True:
                        print("Usuario válido y activo")
                    else:
                        print("Usuario válido pero inactivo")
                else:
                    print("Edad inválida")
            else:
                print("Edad inválida")
        else:
            print("Usuario vacío")
    else:
        print("Usuario nulo")


def calcular_descuento(tipo_cliente, total):
    descuento = 0

    # Complejidad ciclomática elevada
    if tipo_cliente == "A":
        descuento = total * 0.10
    elif tipo_cliente == "B":
        descuento = total * 0.15
    elif tipo_cliente == "C":
        descuento = total * 0.20
    elif tipo_cliente == "D":
        descuento = total * 0.25
    elif tipo_cliente == "E":
        descuento = total * 0.30
    elif tipo_cliente == "F":
        descuento = total * 0.35
    else:
        descuento = 0

    return descuento


def funcion_con_asuntos():
    password = "admin123"   # Credencial hardcodeada (issue de seguridad)
    x = 10
    y = 0

    resultado = 0  # Variable innecesaria

    if y != 0:
        resultado = x / y
    else:
        print("No se puede dividir para cero")

    print("La contraseña es:", password)


def funcion_sin_cobertura():
    # Función que nunca se llama (afecta cobertura)
    print("Esta función no tiene pruebas ni uso")


def main():
    validar_usuario("Juan", 25, True)
    validar_usuario_duplicado("Ana", 30, False)
    print(calcular_descuento("C", 1000))
    funcion_con_asuntos()
    variable_no_usada = 999  # Issue: variable no utilizada


main()








