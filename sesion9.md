<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


### SOLUCION DE CALCULADORA DE RESISTENCIAS


``` java
import java.util.HashMap;
import java.util.Map;

public class CalculadoraResistencias {

    public static void main(String[] args) {
        Map<String, Integer> colores = new HashMap<>();
        colores.put("negro", 0);
        colores.put("marrón", 1);
        colores.put("rojo", 2);
        colores.put("naranja", 3);
        colores.put("amarillo", 4);
        colores.put("verde", 5);
        colores.put("azul", 6);
        colores.put("violeta", 7);
        colores.put("gris", 8);
        colores.put("blanco", 9);

        Map<String, Double> multiplicadores = new HashMap<>();
        multiplicadores.put("negro", 1.0);
        multiplicadores.put("marrón", 10.0);
        multiplicadores.put("rojo", 100.0);
        multiplicadores.put("naranja", 1000.0);
        multiplicadores.put("amarillo", 10000.0);
        multiplicadores.put("verde", 100000.0);
        multiplicadores.put("azul", 1000000.0);
        multiplicadores.put("oro", 0.1);
        multiplicadores.put("plata", 0.01);

        Map<String, Double> tolerancias = new HashMap<>();
        tolerancias.put("marrón", 1.0);
        tolerancias.put("rojo", 2.0);
        tolerancias.put("verde", 0.5);
        tolerancias.put("azul", 0.25);
        tolerancias.put("púrpura", 0.1);
        tolerancias.put("dorado", 5.0);
        tolerancias.put("plateado", 10.0);

        // Valores de las bandas
        String primeraBanda = "verde";
        String segundaBanda = "rojo";
        String terceraBanda = "amarillo";
        String cuartaBanda = "marrón";

        int primerDigito = colores.get(primeraBanda);
        int segundoDigito = colores.get(segundaBanda);
        double multiplicador = multiplicadores.get(terceraBanda);
        double tolerancia = tolerancias.get(cuartaBanda);

        double valor = (primerDigito * 10 + segundoDigito) * multiplicador;
        System.out.println("El valor de la resistencia es " + valor + " ohmios con una tolerancia del " + tolerancia + "%.");
    }
}
```


### SOLUCION DE CALCULADORA DE LA MEDIANA


```JAVA
import java.util.Arrays;

public class CalculadoraMediana {

    public static double calcularMediana(double[] numeros) {
        Arrays.sort(numeros);
        int n = numeros.length;

        if (n % 2 == 0) {
            // El conjunto tiene un número par de elementos
            int medio1 = n / 2 - 1;
            int medio2 = n / 2;
            return (numeros[medio1] + numeros[medio2]) / 2.0;
        } else {
            // El conjunto tiene un número impar de elementos
            int medio = n / 2;
            return numeros[medio];
        }
    }

    public static void main(String[] args) {
        double[] numeros = {5, 2, 9, 1, 5, 6, 3};
        double mediana = calcularMediana(numeros);
        System.out.println("La mediana es: " + mediana);
    }
}



```





