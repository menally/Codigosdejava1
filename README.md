import java.util.Scanner;
public class Main{
    public static void main (String[] args){
        Scanner scanner = new Scanner(System.in);
        System.out.println("Ingresa un numero entero:");
        int numero = scanner.nextInt();
            if (numero > 0 ){
        System.out.println("El numero es positivo");
            } else if (numero < 0) {
                    System.out.println("El numero es negativo");
            } else {
                System.out.println("El numero es cero");
        }
                    System.out.println("-----------------------------");
            System.out.println("Ingresa una hora del dia (0 al 23):");
        int hora = scanner.nextInt();
            if (hora >= 6 && hora <= 11) {
                System.out.println("Buenos dias");
            } else if ( hora >= 12 && hora <= 18){
            System.out.println("Buenas tardes");
            } else if ((hora >= 19 && hora <=23) ||(hora >= 0 && hora <= 5 )){
                    System.out.println("Buenas noches");
            } else {
                System.out.println("Hora incorrecta, por favor ingrese un numero entre el o y 23 ");
            }
            System.out.println("-----------------------------");
          System.out.println("Ingrese un numero entero:");
          numero = scanner.nextInt();
          String resultadoParidad = ( numero % 2== 0) ? "Par": "Impar";
          System.out.println("El numero es:" + resultadoParidad);
          System.out.println();

          System.out.println("-------------------------------");

          System.out.println("Ingresa tu calificacion ");
          int calificacion = scanner.nextInt();
          String resultadoCalificacion = (calificacion <= 60)? "Aprobado":  "Reprobo";
          System.out.println("Estado del alumno " + resultadoCalificacion);
            scanner.close();
        }
      }