# Proyecto Conversion de temperatura

## Descripcion

Este es un programa en Java que permite convertir temperaturas entre Celsius y Fahrenheit. El programa es sencillo de usar, pide la entrada del usuario y realiza la conversión de manera eficiente, mostrando el resultado en pantalla.

## Caracteristicas

Sencillo de usar: Solo se necesita insertar un número (la temperatura) y elegir la conversión que desea realizar (Celsius a Fahrenheit o viceversa).
Mejora futura: La estructura del programa permite agregar más operaciones o conversiones de temperatura fácilmente, o incluso convertirlo en una calculadora más completa.
Simpleza: El código es muy fácil de leer y entender, ideal para principiantes en programación o aquellos que desean una aplicación básica.

## Uso

El uso del programa es simple:

El usuario inserta una temperatura.
Elige la operación que desea realizar:
1. para convertir de Celsius a Fahrenheit.
2. para convertir de Fahrenheit a Celsius.
3. Si la operación es válida, el programa ejecuta la conversión y muestra el resultado. Si la opción es incorrecta, el programa termina sin hacer nada.

## Instalacion

```java
import java.util.Scanner;

public class ConversorTemperaturas {

    // Función que convierte de Celsius a Fahrenheit
    public static double celsiusAFahrenheit(double celsius) {
        return (celsius * 9 / 5) + 32;
    }

    // Función que convierte de Fahrenheit a Celsius
    public static double fahrenheitACelsius(double fahrenheit) {
        return (fahrenheit - 32) * 5 / 9;
    }

    public static void main(String[] args) {
        // Crear un objeto Scanner para recibir la entrada del usuario
        Scanner scanner = new Scanner(System.in);

        // Pedir al usuario que elija la conversión
        System.out.println("Conversor de Temperaturas:");
        System.out.println("1. Convertir de Celsius a Fahrenheit");
        System.out.println("2. Convertir de Fahrenheit a Celsius");
        System.out.print("Selecciona una opción (1 o 2): ");
        int opcion = scanner.nextInt();

        // Realizar la conversión dependiendo de la opción seleccionada
        if (opcion == 1) {
            System.out.print("Introduce la temperatura en Celsius: ");
            double celsius = scanner.nextDouble();
            double fahrenheit = celsiusAFahrenheit(celsius);
            System.out.println(celsius + " grados Celsius son " + fahrenheit + " grados Fahrenheit.");
        } else if (opcion == 2) {
            System.out.print("Introduce la temperatura en Fahrenheit: ");
            double fahrenheit = scanner.nextDouble();
            double celsius = fahrenheitACelsius(fahrenheit);
            System.out.println(fahrenheit + " grados Fahrenheit son " + celsius + " grados Celsius.");
        } else {
            System.out.println("Opción no válida.");
        }

        // Cerrar el escáner
        scanner.close();
    }
}


```
## Lista de tareas

 Explicación de las tareas del programa:

1. Método de Celsius a Fahrenheit y viceversa: El código tiene dos funciones que permiten convertir temperaturas de una unidad a otra.
2. Elegir a qué convertir: El programa pide al usuario que seleccione qué tipo de conversión desea realizar.
3. Dependiendo de la opción, escoge un método u otro: Utiliza un condicional (if-else) para determinar qué función se ejecutará en base a la elección del usuario.
Por hacer a largo plazo
--> Implementar una interfaz gráfica (GUI) para hacerlo más interactivo.
--> Añadir más conversiones de temperatura, como Kelvin.
--> Implementar un control de errores más robusto, por ejemplo, para manejar entradas no válidas (como letras en vez de números).

## Tabla

Característica	Estado
Conversión de Celsius a Fahrenheit	
Conversión de Fahrenheit a Celsius	
Manejo de opciones del usuario	
Validación de entrada (opción no válida)	
Implementación de control de errores	
Interfaz gráfica	
Agregar más conversiones (Kelvin, Rankine, etc.)	

## Enlaces a la web

Estos son enlaces para aprender java

- [PuntoComNoEsUnLenguaje](https://puntocomnoesunlenguaje.blogspot.com/p/teoria_7.html)
... (6 líneas restantes)