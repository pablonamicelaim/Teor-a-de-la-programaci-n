

# Ejercicio combinando estructura condicional y repetitiva (Python).

## ● **Descripción del problema**

El programa está diseñado para calcular el promedio ponderado final de varios estudiantes, tomando en cuenta las calificaciones obtenidas en distintos componentes académicos: ACD, AA, APE y ES. Cada uno de estos componentes tiene un peso específico en la nota final. El programa solicita las notas de cada estudiante, valida que estén en el rango de 0 a 10, calcula los respectivos promedios ponderados y determina una clasificación cualitativa (excelente, buena, regular o deficiente) según el resultado final. Además, registra la suma de todas las notas finales para obtener el promedio general del aula. Al finalizar cada ciclo por estudiante, el programa muestra los ponderados individuales, la nota final y el promedio general acumulado.

## ● **Diagrama de flujo simplificado**

<img width="678" height="1590" alt="image" src="https://github.com/user-attachments/assets/9d33cca5-8534-4a60-bf54-dc5a5f53fde1" />


## ● **Programa**

    # Programa para calcular promedios ponderados de estudiantes

    Suma = 0

    # Número de estudiantes
    Est = int(input("Ingrese el número de estudiantes: "))

    for i in range(1, Est + 1):

    # ---------- Entrada de datos con validación ----------
    def leer_nota(nombre):
        nota = float(input(f"Ingrese la nota que obtuvo en {nombre}: "))
        while nota < 0 or nota > 10:
            print("Error: la calificación debe estar entre 0 y 10.")
            nota = float(input(f"Ingrese nuevamente la nota de {nombre}: "))
        return nota

    # ACD
    ACD1 = leer_nota("ACD1")
    ACD2 = leer_nota("ACD2")

    # AA
    AA1 = leer_nota("AA1")
    AA2 = leer_nota("AA2")

    # APE
    APE1 = leer_nota("APE1")
    APE2 = leer_nota("APE2")

    # ES
    ES1 = leer_nota("ES1")
    ES2 = leer_nota("ES2")

    # ---------- Cálculos de ponderados ----------
    ACD = ((ACD1 + ACD2) / 2) * 0.20
    AA = ((AA1 + AA2) / 2) * 0.20
    APE = ((APE1 + APE2) / 2) * 0.25

    ES1p = ES1 * 0.40
    ES2p = ES2 * 0.60
    ES = (ES1p + ES2p) * 0.35

    NF = ACD + AA + APE + ES

    # ---------- Clasificación ----------
    if NF >= 9:
        print(f"Su nota es {NF:.2f} excelente")
    elif NF >= 7:
        print(f"Su nota es {NF:.2f} buena")
    elif NF >= 5:
        print(f"Su nota es {NF:.2f} regular")
    else:
        print(f"Su nota es {NF:.2f} deficiente")

    Suma += NF

    # ---------- Resultados ----------
    print(f"El promedio del ponderado ACD es {ACD:.2f}")
    print(f"El promedio del ponderado AA es {AA:.2f}")
    print(f"El promedio del ponderado APE es {APE:.2f}")
    print(f"El promedio del ponderado ES es {ES:.2f}")
    print(f"Su nota final de unidad es {NF:.2f}")

    Promedio = Suma / Est
    print(f"El promedio general del aula es: {Promedio:.2f}")
    print("-" * 40)

## ● **Verificación**

<img width="269" height="516" alt="image" src="https://github.com/user-attachments/assets/2693bfe1-0b58-4a17-afcc-6e907569c7f6" />

### [Volver A la Tematicas](../TeoriaU2/unidad2temas.md)
