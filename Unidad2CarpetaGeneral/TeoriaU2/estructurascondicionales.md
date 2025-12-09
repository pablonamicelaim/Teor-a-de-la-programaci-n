
# 🌟 **Tipos de estructuras condicionales y su explicación detallada**

--- 

# **👩‍💻 Contextualización de los Tipos De Estrucuturas:**

## **🔵 Condicional simple**
Esta estructura actúa como un foco puntual dentro del programa: **solo se ejecuta cuando la condición es verdadera**. Si no se cumple, el programa sigue su camino sin hacer nada adicional. Es perfecta cuando se requiere **una única acción dependiente de una condición específica**, como verificar si un número es mayor o si un usuario tiene acceso permitido.

## **🟠 Condicional doble (if–else)**
Funciona como un **cruce de dos caminos**. Si la condición es verdadera, el programa toma un camino; si es falsa, toma el otro. Es útil cuando siempre se debe ejecutar **una de dos posibles acciones**. Por ejemplo, decidir entre “Aprobado” o “Reprobado”, “Encender” o “Apagar”, “Aceptar” o “Rechazar”. Siempre devuelve una respuesta, sin importar cuál sea el resultado.

## **🔺 Condicional múltiple (if–elif–else o switch-case)**
Es la estructura más versátil, como un **menú de opciones**. Permite evaluar **muchas condiciones** y ejecutar la que corresponda a la opción válida. Se utiliza cuando existe más de una respuesta posible, como seleccionar un nivel de dificultad, identificar un día de la semana, elegir una operación matemática o clasificar datos en varias categorías. Le da al programa la capacidad de manejar **diversos escenarios con organización y claridad**.

---

## **Ejercicios**

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

---

## **🟠 Condicional doble (if–else)**

    #include <stdio.h>

    int main() {

    int numero;
    printf("Ingrese un numero:\n");
    scanf("%i", &numero);
    getchar();
    if(numero % 2 == 1){
        printf("El numero %i es impar\n", numero);
    } else {
        printf("El numero %i es par\n",numero);
    } 
    return 0; 
    }
    
## **🔵 Diagrama De Flujo**

<img width="876" height="440" alt="image" src="https://github.com/user-attachments/assets/fed38a08-11ca-4640-a9c5-ac983bc3450f" />

---

## **🔺 Condicional múltiple (switch-case)**

    
    #include <stdio.h>

    int main() {
    int dia; 
        printf("Ingrese el dia de la semana en un numero del 1 al 7:\n", dia);
        scanf("%i", &dia);
        getchar();

        switch(dia) {
            case 1: 
                printf("Es lunes\n");
                break;
            case 2: 
                printf("Es martes\n");
                break;
            case 3: 
                printf("Es miercoles\n");
                break;
            case 4: 
                printf("Es jueves\n");
                break;
            case 5: 
                printf("Es viernes\n");
                break;
            case 6: 
                printf("Es sabado\n");
                break;
            case 7: 
                printf("Es domingo\n");
                break;
            default:
            printf("Numero no valido");
            break;
        }

## **🔵 Diagrama De Flujo**  

<img width="1544" height="470" alt="image" src="https://github.com/user-attachments/assets/8ef82b27-c5d5-4b60-8b0c-176d70cac6cc" />

---

## **🔺 Condicional múltiple (if–elif–else)**

    #include <stdio.h>

    int main() {

    int num1, num2, res;
    char operador;
    printf("Ingrese un numero: ");
    scanf("%i", &num1);
    getchar();

    printf("Ingrese otro numero: ");
    scanf("%i", &num2);
    getchar();

    printf("Ingrese el operador deseado + - * /: ");
    scanf(" %c", &operador);
    getchar();

    if(operador == '+'){
        res = num1 + num2;
        printf("La suma es %i", res);
    }else if (operador == '-')
    {
        res = num1 - num2;
        printf("La resta es de %i", res);

    }else if (operador == '*')
    {
        res = num1 * num2;
        printf("El producto es de %i", res);

    }else if (operador == '/')
    {
        res = num1 / num2;
        printf("El cociente es de %i", res);
    }

    return 0;

    }
    
## **🔵 Diagrama De Flujo**  

<img width="1650" height="1100" alt="image" src="https://github.com/user-attachments/assets/8ebfe2a3-2e3b-4b06-8aa4-2049a5294f84" />

### [Volver A la Tematicas](../TeoriaU2/unidad2temas.md)
