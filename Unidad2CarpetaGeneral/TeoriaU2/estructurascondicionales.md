
# 🌟 **Tipos de estructuras condicionales y su explicación detallada**

--- 

# **👩‍💻 Contextualización de los Tipos De Estrucuturas:**

## **🔵 Condicional simple**
Esta estructura actúa como un foco puntual dentro del programa: **solo se ejecuta cuando la condición es verdadera**. Si no se cumple, el programa sigue su camino sin hacer nada adicional. Es perfecta cuando se requiere **una única acción dependiente de una condición específica**, como verificar si un número es mayor o si un usuario tiene acceso permitido.

## **🟠 Condicional doble (if–else)**
Funciona como un **cruce de dos caminos**. Si la condición es verdadera, el programa toma un camino; si es falsa, toma el otro. Es útil cuando siempre se debe ejecutar **una de dos posibles acciones**. Por ejemplo, decidir entre “Aprobado” o “Reprobado”, “Encender” o “Apagar”, “Aceptar” o “Rechazar”. Siempre devuelve una respuesta, sin importar cuál sea el resultado.

## **🔺 Condicional múltiple (if–elif–else o switch-case)**
Es la estructura más versátil, como un **menú de opciones**. Permite evaluar **muchas condiciones** y ejecutar la que corresponda a la opción válida. Se utiliza cuando existe más de una respuesta posible, como seleccionar un nivel de dificultad, identificar un día de la semana, elegir una operación matemática o clasificar datos en varias categorías. Le da al programa la capacidad de manejar **diversos escenarios con organización y claridad**.

## ** Ejercicios **

## **🔵 Condicional simple**

    #include <stdio.h>

    int main() {

    int num1, num2;
 
    printf("Ingrese un numero:\n");
    scanf("%i", &num1);

    printf("Ingrese un segundo numero:\n");
    scanf("%i", &num2);

    if(num1 > num2){
        printf("El primer numero %i es el mayor\n", num1);
    }
     if(num1 < num2){
        printf("El primer numero %i es el menor\n", num1);
    }   
    if(num1 == num2){
        printf("El primer numero %i es igual a segundo\n", num1);
    }
    return 0;
    }
## **🔵 Diagrama De Flujo**

<img width="838" height="880" alt="image" src="https://github.com/user-attachments/assets/72d6a882-b6f5-413a-bd03-58c3419f1266" />
