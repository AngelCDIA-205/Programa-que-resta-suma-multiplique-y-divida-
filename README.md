# Programa-que-resta-suma-multiplique-y-divida-
def sumar(a, b):
    return a + b

def restar(a, b):
    return a - b

def multiplicar(a, b):
    return a * b

def dividir(a, b):
    if b == 0:
        return "Error: División por cero"
    return a / b

def main():
    print("Calculadora simple:")
    print("1. Sumar")
    print("2. Restar")
    print("3. Multiplicar")
    print("4. Dividir")

    opcion = input("Elige una opción (1/2/3/4): ")
    a = float(input("Ingresa el primer número: "))
    b = float(input("Ingresa el segundo número: "))

    if opcion == "1":
        resultado = sumar(a, b)
    elif opcion == "2":
        resultado = restar(a, b)
    elif opcion == "3":
        resultado = multiplicar(a, b)
    elif opcion == "4":
        resultado = dividir(a, b)
    else:
        resultado = "Opción inválida"

    print("Resultado:", resultado)

if __name__ == "__main__":
    main()
