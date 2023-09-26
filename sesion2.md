<!-- No borrar o modificar -->
[Inicio](./index.md)


# ACTIVIDAD 2

1. Programa para calcular la hipotenusa de un triángulo rectángulo

 ### SOLUCIÓN

```JAVA
public class HipotenusaTriangulo1 {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese el valor del primer cateto: ");
            double cateto1 = scanner.nextDouble();
            
            System.out.print("Ingrese el valor del segundo cateto: ");
            double cateto2 = scanner.nextDouble();
            
            double hipotenusa = Math.sqrt(Math.pow(cateto1, 2) + Math.pow(cateto2, 2));
            System.out.println("La hipotenusa del triángulo es: " + hipotenusa);
        }
    }
    }
```

2. Programa para determinar si un número es par o impar:

### SOLUCIÓN 

```JAVA
public class Java1 {
    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese un número: ");
            int numero = scanner.nextInt();
            
            if (numero % 2 == 0) {
                System.out.println("El número es par.");
            } else {
                System.out.println("El número es impar.");
            }
        }
    }
    }
```

3. Programa para calcular el tercer ángulo de un triángulo:

### SOLUCIÓN

```JAVA
public class TercerAnguloTriangulo {
    
        public static void main(String[] args) {
            try (Scanner scanner = new Scanner(System.in)) {
                System.out.print("Ingrese el valor del primer ángulo: ");
                int angulo1 = scanner.nextInt();
                
                System.out.print("Ingrese el valor del segundo ángulo: ");
                int angulo2 = scanner.nextInt();
                
                if (angulo1 > 0 && angulo1 < 180 && angulo2 > 0 && angulo2 < 180) {
                    int tercerAngulo = 180 - (angulo1 + angulo2);
                    System.out.println("El valor del tercer ángulo es: " + tercerAngulo);
                } else {
                    System.out.println("Los valores ingresados no son ángulos válidos.");
                }   }
    }
}
```

4. Programa para calcular el promedio de tres números:

### SOLUCIÓN

```JAVA 
public class PromedioTresNumeros {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese el primer número: ");
            double numero1 = scanner.nextDouble();
            
            System.out.print("Ingrese el segundo número: ");
            double numero2 = scanner.nextDouble();
            
            System.out.print("Ingrese el tercer número: ");
            double numero3 = scanner.nextDouble();
            
            double promedio = (numero1 + numero2 + numero3) / 3;
            System.out.println("El promedio de los tres números es: " + promedio);
        }
    }
}
```

5. Programa para calcular la longitud de una cadena de texto:

### SOLUCIÓN

```JAVA 
public class LongitudCadena {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese una cadena de texto: ");
            String texto = scanner.nextLine();
            
            int longitud = texto.length();
            System.out.println("La longitud de la cadena es: " + longitud);
        }
    }
    }
```

6. Programa para calcular el área de un triángulo:

### SOLUCIÓN

```JAVA
public class AreaTriangulo {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese la base del triángulo: ");
            double base = scanner.nextDouble();
            
            System.out.print("Ingrese la altura del triángulo: ");
            double altura = scanner.nextDouble();
            
            double area = (base * altura) / 2;
            System.out.println("El área del triángulo es: " + area);
        }
    }
    } 
```

7. Programa para calcular la raíz cuadrada de un número:

### SOLUCIÓN

```JAVA

public class RaizCuadrada {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese un número: ");
            double numero = scanner.nextDouble();
            
            double raizCuadrada = Math.sqrt(numero);
            System.out.println("La raíz cuadrada del número es: " + raizCuadrada);
        }
    }
}

```

8. Programa para calcular el máximo común divisor (MCD) de dos números:

### SOLUCIÓN

```JAVA 

public class MaximoComunDivisor {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese el primer número: ");
            int numero1 = scanner.nextInt();
            
            System.out.print("Ingrese el segundo número: ");
            int numero2 = scanner.nextInt();
            
            int mcd = calcularMCD(numero1, numero2);
            System.out.println("El máximo común divisor de los dos números es: " + mcd);
        }
    }
}
```
9. Programa para imprimir una cadena de texto en orden inverso:

### SOLUCIÓN

```JAVA
import java.util.Scanner;

public class CadenaInversa {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese una cadena de texto: ");
        String texto = scanner.nextLine();

        String textoInverso = "";
        for (int i = texto.length() - 1; i >= 0; i--) {
            textoInverso += texto.charAt(i);
        }

        System.out.println("La cadena en orden inverso es: " + textoInverso);

        scanner.close();
    }
}
```

10. Programa para calcular el área de un rectángulo:

### SOLUCIÓN

```JAVA

public class AreaTriangulo {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Ingrese la base del triángulo: ");
            double base = scanner.nextDouble();
            
            System.out.print("Ingrese la altura del triángulo: ");
            double altura = scanner.nextDouble();
            
            double area = (base * altura) / 2;
            System.out.println("El área del triángulo es: " + area);
        }
    }
}
```






