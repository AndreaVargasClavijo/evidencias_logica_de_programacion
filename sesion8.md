<!-- No borrar o modificar -->
[Inicio](./index.md)

# ACTIVIDAD 8

Implementar los siguientes métodos:

- Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

### SOLUCION 

``` JAVA

public class Funciones1 {

    public static void main(String[] args) {
        int n1 = 10;
        int n2 = 5;
        int mayor = numeroMayor(n1, n2);
        
        System.out.println("el numero mayor es:"  + mayor);
                
        
    }
    
    public static int numeroMayor(int n1, int n2) {
        if (n1 > n2){
            return n1;
        } else {
            return n2;
        }
    }
   }
```

- Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.


### SOLUCION 


``` JAVA 
public class Funciones2 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("ingrese una frase: ");
        
        String cadena = sc.nextLine();
        
        int numeroVocales = contadorVocales(cadena);
        
        System.out.println("el numero de vocales es:" + numeroVocales);
        
        sc.close();
    }

    public static int contadorVocales(String cadena) {
        int contador = 0;
        String vocales = "aeiouAEIOU";

        for (int i = 0; i < cadena.length(); i++) {
              char caracter = cadena.charAt(i);
        
        
        if (vocales.indexOf(caracter) != -1) {
            contador++;
        }
    }
        return contador;
    }

}

```

- Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

### SOLUCION 

``` JAVA
public class Funcion3 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("ingrese una frase con inicial mayuscula");

        String cadena = sc.nextLine();

        String resultado = cadena2(cadena);

        System.out.println("la nueva Frase es:" + resultado);
        
        sc.close();

    }

    public static String cadena2(String cadena) {

        StringBuilder resultado = new StringBuilder();

        for (int i = 0; i < cadena.length(); i++) {
            char caracter = cadena.charAt(i);

            if (Character.isUpperCase(caracter)) {
                resultado.append(Character.toLowerCase(caracter));
            } else if(Character.isLowerCase(caracter)){
                resultado.append(Character.toUpperCase(caracter));
            } else {
                resultado.append(caracter);
            }
        }
        return resultado.toString();
    }
}
```

- Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

### SOLUCION 

``` JAVA
public class Funciones4 {

    public static void main(String[] args) {
        Scanner sc =new Scanner(System.in);
        
        System.out.println("ingrese su frase");
        
        String cadena = sc.nextLine();
        
        int palabras = npalabras(cadena);
        
        System.out.println("el numero de palabras es " + palabras);
    }
    
    public static int npalabras(String cadena){
        String[] palabras = cadena.split("\\s+");
        return palabras.length;
    }
}

```

- Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

``` JAVA
public class Funciones5 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("ingrese una frase");

        String cadena = sc.nextLine();

        String resul = cadenaOrdenAlfabetico(cadena);

        System.out.println("las palabras ordenadas son " + resul);
    }

    public static String cadenaOrdenAlfabetico(String cadena) {
        String[] palabras = cadena.split("\\s+");

        Arrays.sort(palabras);
        return String.join(" ", palabras);

    }
}
```









