<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


<!-- Su documentación aquí -->

### SOLUCION DE NUMEROS REPETIDOS

```JAVA
public class Ejercicio1 {

    public static void main(String[] args) {
        // Declaramos un conjunto de números enteros
        int[] numeros = {1, 2, 3, 4, 5, 2, 1};

        // Creamos una variable para almacenar el número que aparece más de una vez
        int numeroRepetido = 0;

        // Recorremos el conjunto de números
        for (int i = 0; i < numeros.length; i++) {
            // Comprobamos si el número actual ya ha aparecido
            for (int j = 0; j < i; j++) {
                if (numeros[i] == numeros[j]) {
                    // El número actual ya ha aparecido
                    numeroRepetido = numeros[i];
                    break;
                }
            }
        }

        // Si el número repetido es distinto de 0, lo imprimimos
        if (numeroRepetido != 0) {
            System.out.println("El número repetido es: " + numeroRepetido);
        } else {
            // No hay ningún número repetido
            System.out.println("No hay ningún número repetido");
        }
    }
}
```


### SOLUCION BINARIOS A DECIMAL

```JAVA
import java.util.Scanner;

public class BinarioADecimal {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Ingresa un número binario: ");
        String numeroBinario = scanner.nextLine();

        int longitud = numeroBinario.length();
        int resultado = 0;

        for (int i = 0; i < longitud; i++) {
            char bit = numeroBinario.charAt(i);
            int valorBit = Character.getNumericValue(bit);

            if (valorBit != 0 && valorBit != 1) {
                System.out.println("¡Error! El número no es binario.");
                return;
            }

            int potencia = longitud - i - 1;
            resultado += valorBit * Math.pow(2, potencia);
        }

        System.out.println("El equivalente decimal es: " + resultado);
    }
}

```



