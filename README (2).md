# TestMethods

## Descripción
Este proyecto implementa la clase `TestMethods` en Java, una biblioteca de utilidades que
proporciona funcionalidades para cálculos matemáticos, manejo de colecciones y procesamiento de texto.
La clase incluye métodos para realizar operaciones como cálculo factorial, generación de números aleatorios,
manipulación de listas y análisis de frecuencia de caracteres.

## Características
- Programa ejecutable independiente
- 8 métodos implementados
- Manejo de colecciones y estructuras de datos

## Métodos Implementados
### `main`
```java
void main(String[] args)
```
Método principal que inicia la ejecución del programa.

Parámetros:
- args (String[])

Ejemplo de uso:
```java
public class TestMethods {
    public static void main(String[] args) {
        // Crear instancia de la clase
        TestMethods programa = new TestMethods();

        // Ejemplo de uso de varios métodos
        programa.printMessage("Hola Mundo!");
        int suma = programa.addNumbers(5, 3);
        System.out.println("La suma es: " + suma);
    }
}
```

### `printMessage`
```java
void printMessage(String message)
```
Muestra información en la consola.

Parámetros:
- message (String)

Ejemplo de uso:
```java
programa.printMessage("ejemplo");
```

### `addNumbers`
```java
int addNumbers(int a, int b)
```
Realiza la suma de dos números y retorna el resultado.

Parámetros:
- a (int)
- b (int)

Retorna: int

Ejemplo de uso:
```java
int resultado = programa.addNumbers(5, 5);
System.out.println("Suma: " + resultado);
```

### `getRandomNumber`
```java
int getRandomNumber()
```
Genera y retorna un número aleatorio.

Retorna: int

Ejemplo de uso:
```java
int resultado = programa.getRandomNumber();
System.out.println("Número aleatorio generado: " + resultado);
```

### `getNames`
```java
List<String> getNames()
```
Obtiene y retorna una lista de nombres.

Retorna: List<String>

Ejemplo de uso:
```java
List<String> nombres = programa.getNames();
System.out.println("Lista de nombres: " + nombres);
```

### `calculateFactorial`
```java
int calculateFactorial(int n)
```
Calcula el factorial de un número dado.

Parámetros:
- n (int)

Retorna: int

Ejemplo de uso:
```java
int resultado = programa.calculateFactorial(5);
System.out.println("Factorial de 5: " + resultado);
```

### `reverseList`
```java
List<String> reverseList(List<String> list)
```
Invierte el orden de los elementos en una lista.

Parámetros:
- list (List<String>)

Retorna: List<String>

Ejemplo de uso:
```java
List<String> listaOriginal = Arrays.asList("A", "B", "C");
List<String> resultado = programa.reverseList(listaOriginal);
System.out.println("Lista invertida: " + resultado);
```

### `countCharacters`
```java
Map<Character, Integer> countCharacters(String input)
```
Cuenta la frecuencia de cada carácter en una cadena de texto.

Parámetros:
- input (String)

Retorna: Map<Character, Integer>

Ejemplo de uso:
```java
Map<Character, Integer> resultado = programa.countCharacters("ejemplo");
System.out.println("Frecuencia de caracteres: " + resultado);
```

## Imports necesarios
```java
import java.util.ArrayList;
import java.util.Arrays;
import java.util.Collections;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Random;
```

## Ejemplo de uso completo
```java
public class TestMethodsDemo {
    public static void main(String[] args) {
        // Crear instancia de TestMethods
        TestMethods programa = new TestMethods();

        // Ejemplo de mensaje y operaciones matemáticas
        programa.printMessage("Iniciando demostracion...");
        int suma = programa.addNumbers(10, 5);
        System.out.println("Suma: " + suma);

        // Ejemplo de número aleatorio y factorial
        int aleatorio = programa.getRandomNumber();
        System.out.println("Numero aleatorio: " + aleatorio);
        int factorial = programa.calculateFactorial(5);
        System.out.println("Factorial de 5: " + factorial);

        // Ejemplo de manejo de listas
        List<String> nombres = programa.getNames();
        System.out.println("Lista original: " + nombres);
        List<String> invertida = programa.reverseList(nombres);
        System.out.println("Lista invertida: " + invertida);

        // Ejemplo de análisis de texto
        String texto = "programacion";
        Map<Character, Integer> frecuencia = programa.countCharacters(texto);
        System.out.println("Frecuencia de caracteres: " + frecuencia);
    }
}
```

## Requisitos
- Java JDK 8 o superior
- Compilador de Java (javac)

## Instalación
1. Descarga `TestMethods.java`
2. Compila el código:
```bash
javac TestMethods.java
```
3. Ejecuta el programa:
```bash
java TestMethods
```

## Autor
- [Tu Nombre]

## Licencia
Este proyecto está bajo la Licencia MIT.
