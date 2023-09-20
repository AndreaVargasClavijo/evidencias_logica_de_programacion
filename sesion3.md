<!-- No borrar o modificar -->
[Inicio](./index.md)

# ACTIVIDAD 3


1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

### SOLUCIÓN

``` JAVA COPY
package com.mycompany.lpn1;

import java.util.Scanner;
/**
 *
 * @author ANDREA
 */
public class LPN1 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner (System.in);
        
        System.out.println("ingrese el primer número: ");
        int num1 = scanner.nextInt();
        
        System.out.println("ingrese el segundo número: ");
        int num2 = scanner.nextInt();
        
        int suma = (num1 + num2);
        int multiplicacion = (num1 * num2); 
        
        System.out.println("la suma es: " + suma);
        System.out.println("la multiplicación es: " + multiplicacion);
        
        
        System.out.println("el resultado de la suma es: " + suma + " y de la multiplicación es: " + multiplicacion);
        
        scanner.close();
    }
}

```

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

### SOLUCIÓN

``` JAVA COPY
package com.mycompany.lpn2;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class LPN2 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner (System.in);
        
        System.out.println("ingrese el primer número: ");
        int num1 = scanner.nextInt();
        
        System.out.println("ingrese el segundo número: ");
        int num2 = scanner.nextInt();
        
        int resta = (num1 - num2);
        int division = (num1 / num2); 
        
        System.out.println("la resta es: " + resta);
        System.out.println("la division es: " + division);
        
        
        System.out.println("el resultado de la resta es: " + resta + " y de la división es: " + division);
        
        scanner.close();
    }
}
```
3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

### SOLICIÓN

``` JAVA COPY
package com.mycompany.operacionescombinadas;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class OperacionesCombinadas {

    public static void main(String[] args) {
          Scanner scanner = new Scanner (System.in);
        
        System.out.println("ingrese el primer número: ");
        int num1 = scanner.nextInt();
        
        System.out.println("ingrese el segundo número: ");
        int num2 = scanner.nextInt();
        
        System.out.println("ingrese el segundo número: ");
        int num3 = scanner.nextInt();
        
        int suma = (num1 + num2 + num3);
        int combinada = (num1 * num2 / num3); 
        
        System.out.println("la suma es: " + suma);
        System.out.println("el resultado de la multiplicacion y division es: " + combinada);
        
        
        System.out.println("el resultado de la suma es: " + suma + " y de la operacion combinada es: " + combinada);
        
        scanner.close();
    }
}
```
4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

### SOLUCIÓN 

``` JAVA COPY
package com.mycompany.decimales;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class Decimales {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double num1;
        double num2;
        
        System.out.print("Dame el valor del primer número: ");
        num1 = scanner.nextDouble();
        System.out.print("Dame el valor del segundo número: ");
        num2 = scanner.nextDouble();

        System.out.println("La suma de estos números es " + (num1 + num2));
        System.out.println("La resta de estos números es " + (num1 - num2));
        System.out.println("La multiplicación de estos números es " + (num1 * num2));
        System.out.println("La división de estos números es " + ((double)num1 / (double)num2));

    }
}
```

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

### SOLUCIÓ

``` JAVA COPY
package com.mycompany.incrementodecremento;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class IncrementoDecremento {

    public static void main(String[] args) {
         Scanner scanner = new Scanner (System.in);
         
        
        System.out.println("ingrese el número: ");

      
        int num1 = scanner.nextInt();
        
        System.out.println("el numero en incremento es:" + ++num1);
        
        num1 = num1--;
        System.out.println("el numero en decremento es:" +   (num1--));
        
        scanner.close();        
        
    }
}

```

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

### SOLUCIÓN

``` JAVA COPY
package com.mycompany.asigancioncompuesta;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class AsigancionCompuesta {

    public static void main(String[] args) {
Scanner scanner = new Scanner (System.in);
        


        int num1 = 10; 
        
        System.out.println("ingrese el número a sumar: ");
        int num2 = scanner.nextInt();
        
        int sumaCompuesta = (num1 += num2);
        
        System.out.println("la suma es: " + sumaCompuesta);
        
        
        System.out.println("el resultado de la suma es: " + sumaCompuesta);
        
        scanner.close();    }
}
```

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

### SOLUCIÓN

``` JAVA COPY
package com.mycompany.operadoreslogicos;

/**
 *
 * @author ANDREA
 */
public class OperadoresLogicos {

    public static void main(String[] args) {
        int edad = 18;
        int peso = 55;
        boolean persona = true;
        

        boolean resultado1 = (edad > 30) || persona;
        boolean resultado2 = persona && (peso < 50);
        boolean resultado3 = !persona;

        System.out.println("El resultado 1 es: " + resultado1);
        System.out.println("El resultado 2 es: " + resultado2);
        System.out.println("El resultado 3 es: " + resultado3);
       
       
        
    }
}
```

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.

### SOLUCIÓN 

``` JAVA  COPY
package com.mycompany.operadorternario;

import java.util.Scanner;

/**
 *
 * @author ANDREA
 */
public class OperadorTernario {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("escribe el numero:");
        double num1 = scanner.nextDouble();
        
        if (num1 >= 0) {
            System.out.println("el numero es positivo");
        } else if (num1 < 0) {
        System.out.println("el numero es negativo");
    }
    }
}
```








