<!-- No borrar o modificar -->
[Inicio](./index.md)

# ACTIVIDAD 4

``` JAVA 
// Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;
```

1. Determinar si el estudiante es mayor de edad y tiene un estado activo.
2. Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.
3. Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.
4. Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.
5. Mostrar toda la información del estudiante si está matriculado en el Cesde.
6. Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.
7. Determinar la cantidad de beca que recibe el estudiante según su promedio:
0.0 - 3.4: El estudiante no recibe beca.
3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
4.5 - 5.0: El estudiante recibe una beca completa.

``` JAVA 
public class Lpn {

    public static void main(String[] args) {
        String nombre = "Juan Pérez";
        String apellido = "González";
        String identificación = "1000000001";
        String correo = "juan.perez@ejemplo.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";

        int edad = 20;
        boolean esActivo = true;
        boolean becado = false;
        char género = 'M';
        double promedio = 4.5;
        int semestre = 2;
//** ejercicio 1
        if (edad >= 18 && esActivo) {
            System.out.println("el estudiante es mayor de edad y esta activo");
        } else {
            System.out.println("el estudiante no es mayor de edad y no esta activo");
        }
//** ejercicio 2
        if (becado != false && !carrera.equals("Desarrollo de Software")) {
            System.out.println("el estudiante no es becado y tiene una carrera en desarrollo de software");
        } else {
            System.out.println("el estudiante es becado y no tiene carrera de software");
        }
//ejercicio 3
        if (semestre <= 3 && esActivo) {
            System.out.println("el estudiante esta en segundo y semestre esta activo");
        } else {
            System.out.println("el estudiante esta en un semestre superior esta activo");
        }
//**ejercicio 4
        if (promedio >= 4.0 && carrera.equals("Desarrollo de Software")) {
            System.out.println("el estudiante tiene promedio superior de 4.0 y tiene carrera de software");
        } else {
            System.out.println("el estudiante tiene pormedio inferior de 4.0");
        }
//** ejercicio 5
        if (universidad.equals("Cesde")) {
            System.out.println("el nombre es: " + nombre);
            System.out.println("el apellido es: " + apellido);
            System.out.println("la cedula ciudadania es: " + identificación);
            System.out.println("el correo es: " + correo);
            System.out.println("la edad es: " + edad);
            System.out.println("el genero es: " + género);

        } else {
            System.out.println("no se encuentra en la base de datos");
        }
//ejercicio 6
        if (promedio >= 4.0 && universidad.equals("Cesde") && esActivo) {
            System.out.println("se da beca de 50% a estudiante");
        } else {
            System.out.println("no cumple para la beca");
        }
//ejercicio 7
        if (promedio >= 0.0 && promedio <= 3.4) {
            System.out.println("no recibe beca");
        } else if (promedio >= 3.5 && promedio <= 3.9) {
            System.out.println("aplica a beca parcial de 25%");
        } else if (promedio >= 4.0 && promedio <= 4.4) {
            System.out.println("recibe beca del 50%");
        } else if (promedio >= 4.5 && promedio <= 5.0) {
            System.out.println("se da beca completa");
        }
// 3 ejercicios adicionales
// 1 ejercicio adicional notificar por correo beca brindada.

        if (promedio >= 4.5 && promedio <= 5.0 && correo.equals("juan.perez@ejemplo.com")) {
        System.out.println("se envia notificación al correo de beca ganadora");
        } else {
        System.out.println("se envia por whatsapp");
        }
// 2 ejercicio adicional: invitacion partido de futbol en la universidad. 

         if (edad >= 20 && género == 'M') {
         System.out.println("invitacion a Juan a partido de futbol");
         } else {
         System.out.println("no se convoca a la actividad");
         }
// 3 ejercicio adicional: reconocimiento de honor
        if (promedio >= 4.5 && semestre == 2) {
        System.out.println("se da reconocimiento a" + nombre + apellido + "por su perseverancia en el aprendizaje");
        }
    }
}

```








