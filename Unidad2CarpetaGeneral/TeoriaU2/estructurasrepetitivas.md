# 🌟 **Tipos de estructuras repetitivas y su explicación detallada**

--- 

# **👩‍💻 Contextualización de los Tipos De Estrucuturas:**

## **🔁 Bucle Mientras (while)**

Funciona como un semáforo que permanece verde mientras la condición sea verdadera. El ciclo se repite una y otra vez hasta que la condición deje de cumplirse. Es ideal cuando no sabemos cuántas veces se repetirá el proceso, como leer datos hasta que el usuario escriba “0”, o sumar números mientras sean positivos. El control del ciclo depende totalmente de la condición.

## **🔄 Bucle Repetir…Hasta Que (do–while en algunos lenguajes)**

Este bucle garantiza que la acción se ejecute al menos una vez, sin importar la condición. Es como probar una comida antes de decidir si seguir comiendo: primero se ejecuta, luego se verifica si se debe continuar o detener. Se usa cuando la primera ejecución es obligatoria, como pedir una contraseña hasta que sea válida.

## **🔃 Bucle Para (for)** 

Es el más ordenado y predecible, como una cuenta regresiva programada. Se utiliza cuando ya se conoce la cantidad de repeticiones, como recorrer una lista, imprimir una serie del 1 al 10, o procesar a un número fijo de estudiantes. Define inicio, final y el paso del contador, lo que lo convierte en el ciclo más estructurado y fácil de controlar.

## ** Ejercicios **

## **🔁 Bucle Mientras (while)**
    
    #include<stdio.h>

    int main()
    {
    int n, c, acumulador;
    c = 0;
    
    printf("Ingrese un numero: ");
    scanf("%i", &n);
    
    while(n >= 1){
        printf("Ingrese un numero: ");
        scanf("%i", &n);
        c = c + 1;
    }    
    printf("haz ingresado %i números positivos", c);
       return 0;
    }

## **🔵 Diagrama De Flujo**

<img width="536" height="710" alt="image" src="https://github.com/user-attachments/assets/d71d57aa-00c6-464c-a63d-8f15be6f8da4" />

## **🔄 Bucle Repetir…Hasta Que (do–while en algunos lenguajes)**

    #include <stdio.h>

    int main() {

    int numerador, denominador, r;

    printf("Ingrese el numerador:\n");
    scanf("%i", &numerador);
    getchar();

    // Ciclo para evitar denominador igual a 0
    do {
        printf("Ingrese el denominador:\n");
        scanf("%i", &denominador);
        getchar();

    } while (denominador == 0);

    r = numerador / denominador;

    printf("El resultado de su division es %i\n", r);

    return 0;
    }

## **🔵 Diagrama De Flujo**

<img width="864" height="770" alt="image" src="https://github.com/user-attachments/assets/e38dffed-22ed-42bd-ac39-54fbe9c523d8" />

## **🔃 Bucle Para (for)** 

      int horas, dias;

    for(dias = 1; dias <=365; dias++){
        
        for(horas = 1; horas <=24; horas++){
            printf("Tempera de la hora %i del dia %i\n", horas, dias);
            
        }
    }
    return 0;
    }

## **🔵 Diagrama De Flujo**

<img width="922" height="368" alt="image" src="https://github.com/user-attachments/assets/08fa64d6-8622-4a53-93e6-9da02b5360c2" />

### [Volver A la Tematicas](../TeoriaU2/unidad2temas.md)
