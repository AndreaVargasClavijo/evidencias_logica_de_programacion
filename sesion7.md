<!-- No borrar o modificar -->
[Inicio](./index.md)

## ACTIVIDAD 7


Ejecicios Array - ArrayList



- En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.


### Ejemplo Array

``` java
public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
```

### Ejemplo Array list

``` java
public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }

  public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}

```

- Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.


## ARRAY 

``` JAVA
public class Array {

    public static void main(String[] args) {
        Scanner entrada = new Scanner(System.in);
        String [] nombresInvitadas = new String[5];
        
        nombresInvitadas[0] = "paola";
        nombresInvitadas[1] = "veronica";
        nombresInvitadas[2] = "andrea";
        nombresInvitadas[3] = "tatiana";
        nombresInvitadas[4] = "eliana";
        
    
        
        System.out.println("las invitadas a pijamada son:" + Arrays.toString(nombresInvitadas)); 
        
        
        System.out.println("ingrese a los nuevos invitados:");
        String nuevosInvitados = entrada.nextLine();
        
       System.out.println("el nuevo invitado es: " + nuevosInvitados);
        
    }
}
```

## ARRAYLIST 

``` JAVA
public class Array_list {

    public static void main(String[] args) {
        Scanner entrada = new Scanner(System.in);

        ArrayList<String> color = new ArrayList<>();

        color.add("rojo");
        color.add("amarillo");
        color.add("azul");
        color.add("negro");
        color.add("blanco");

        System.out.println("los colores son:" + color);

        System.out.println("el color mas usado es " + color.get(3));

        
        color.remove(3);
        
        System.out.println(color);
        
        System.out.println("ingrese nuevo color:");
        String nuevoColor = entrada.nextLine();
        
       System.out.println("el nuevo color es: " + nuevoColor);
    }

}

```



