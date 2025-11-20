## Resolución De Ejercicios: 

## 1. Ejercicio

### Algoritmo en Pseudocogido

Algoritmo convertir_metros
		Definir metros, km, cm, mm Como Real
		
		Escribir "Ingrese la cantidad en metros:"
		Leer metros
		
		km = metros / 1000
		cm = metros * 100
		mm = metros * 1000
		
		Escribir "Kilómetros: ", km
		Escribir "Centímetros: ", cm
		Escribir "Milímetros: ", mm
FinAlgoritmo

### Diagrama de Flujo

<img width="398" height="626" alt="image" src="https://github.com/user-attachments/assets/3a8d6336-b6bc-482a-98f6-5d5d3cd77652" />

### Lenguaje C 

#include <stdio.h>

int main() {
    float metros, km, cm, mm;

    printf("Ingrese la cantidad en metros: ");
    scanf("%f", &metros);

    km = metros / 1000;
    cm = metros * 100;
    mm = metros * 1000;

    printf("Kilometros: %.3f\n", km);
    printf("Centimetros: %.2f\n", cm);
    printf("Milimetros: %.2f\n", mm);

    return 0;
}

### Prueba De Escritorio 

<img width="693" height="180" alt="image" src="https://github.com/user-attachments/assets/a17e6eb3-12dd-4eb8-86b3-dcd720f312dd" />

## 2. Ejercicio

### Algoritmo en Pseudocodigo

Algoritmo aceleracion
    Definir vi, vf, t, a Como Real

    Escribir "Ingrese la velocidad inicial (m/s):"
    Leer vi

    Escribir "Ingrese la velocidad final (m/s):"
    Leer vf

    Escribir "Ingrese el tiempo (s):"
    Leer t

    a = (vf - vi) / t

    Escribir "La aceleracion es: ", a, " m/s^2"
FinAlgoritmo

### Diagrama De Flujo

<img width="444" height="616" alt="image" src="https://github.com/user-attachments/assets/d56b6fde-2ae5-4641-953e-509f3353a95f" />

### Lenguaje C 

#include <stdio.h>

int main() {
    float vi, vf, t, a;

    printf("Ingrese velocidad inicial (m/s): ");
    scanf("%f", &vi);

    printf("Ingrese velocidad final (m/s): ");
    scanf("%f", &vf);

    printf("Ingrese el tiempo (s): ");
    scanf("%f", &t);

    a = (vf - vi) / t;

    printf("La aceleracion es: %.3f m/s^2\n", a);

    return 0;
}

### Prueba de Escritorio

<img width="656" height="195" alt="image" src="https://github.com/user-attachments/assets/8ab6b8d7-cf4d-406c-86de-11b8403e4cfa" />

 ## 3. Ejercicio

 ### Algoritmo en Pseudocodigo

 Algoritmo distancia_puntos
    Definir x1, y1, x2, y2, d Como Real

    Escribir "Ingrese x1:"
    Leer x1

    Escribir "Ingrese y1:"
    Leer y1

    Escribir "Ingrese x2:"
    Leer x2

    Escribir "Ingrese y2:"
    Leer y2

    d = raiz((x2 - x1)^2 + (y2 - y1)^2)

    Escribir "La distancia es: ", d
FinAlgoritmo

### Diagrama de Flujo 

<img width="396" height="626" alt="image" src="https://github.com/user-attachments/assets/80804fe6-307f-4037-9d73-34cf42aad948" />

### Lenguaje C 

#include <stdio.h>
#include <math.h>

int main() {
    float x1, y1, x2, y2, d;

    printf("Ingrese x1: ");
    scanf("%f", &x1);

    printf("Ingrese y1: ");
    scanf("%f", &y1);

    printf("Ingrese x2: ");
    scanf("%f", &x2);

    printf("Ingrese y2: ");
    scanf("%f", &y2);

    d = sqrt(pow(x2 - x1, 2) + pow(y2 - y1, 2));

    printf("La distancia es: %.3f\n", d);

    return 0;
}

### Prueba de Escritorio

<img width="642" height="237" alt="image" src="https://github.com/user-attachments/assets/c98cb608-5e7b-42b2-87ae-c2fa9a042d86" />





