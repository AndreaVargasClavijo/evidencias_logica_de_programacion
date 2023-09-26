<!-- No borrar o modificar -->
[Inicio](./index.md)

 # ACTIVIDAD 5 

 ## Ejercicios - while

1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

### SOLUCIÓN 

``` JAVA
public class While1 {

    public static void main(String[] args) {
        int num;
        
        System.out.println("digite su numero");
        
        
        Scanner resultado = new Scanner (System.in);
        
        num = resultado.nextInt();
        
        int multiplicacion = 1;
        
        while (multiplicacion <= 10) {
            System.out.println(num +  " x" + multiplicacion + "=" + num * multiplicacion);
            multiplicacion++;
        }
        
    }
} 
```

2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

### SOLUCIÓN

``` JAVA
public class While2 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("ingrese la frase.");

        String cadena = scanner.nextLine();

        int num = 0;

        int contadorNumeros = 0;

        while (num < cadena.length()) {
            char numero = cadena.charAt(num);
            if (Character.isDigit(numero)) {
                contadorNumeros++;
            }
            num++;
        }
        System.out.println("la frase tiene " + contadorNumeros + " numeros");
    }
}
```

## Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

### SOLUCIÓN 

``` JAVA
public class DoWhile1 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int numero = 1;

        System.out.println("ingrese un numero");
        int num = scanner.nextInt();

        do {
            System.out.println(numero);
            numero++;
        } while (numero <= 100 && num >= 0);
    }
}

```
2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

### SOLUCIÓN 

``` JAVA
public class DoWhile2 {

    @SuppressWarnings("empty-statement")
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("ingrese su numero para multiplicar: ");

        int num = scanner.nextInt();

        int multiplicacion = 1;

        do {
            System.out.println(num + " x" + multiplicacion + "=" + num * multiplicacion);
            multiplicacion++;
        } while (num != 0 && multiplicacion <= 10);
        
    }
}
```

## Ejercicios - for

1. Imprimir los números impares del 1 al 50.

### SOLUCIÓN 

``` JAVA
public class For1 {

    public static void main(String[] args) {
 
        for (int i=1; i<50; i+=2) {
            System.out.println(i);
        }
    }
}  
```

2. Imprimir los números primos del 1 al 100.

### SOLUCIÓN

``` JAVA
public class For2 {

    public static void main(String[] args) {
        int prueba = 100;

        for (int num = 1; num <= prueba; num++) {
            int div = 0;
            for (int x = 1; x <= num / 2; x++) {
                if (num % x == 0) {
                    div += 2;

                }
                if (div > 2) {
                    break;
                }

            }
            if (div == 2) {
                System.out.println(num);

            }
        }

    }
} 
``` 







