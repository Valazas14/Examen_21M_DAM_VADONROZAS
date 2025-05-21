package REPOSITORIOS;

public class EXAMEN_21M_PRIMO {
    public static void main(String[] args) {
        System.out.println("Buenos días Ceinmark, soy Marta Gómez");
        
        java.util.Scanner scanner = new java.util.Scanner(System.in);
        System.out.print("Introduce un número para averiguar si es primo o no: ");
        int numero = scanner.nextInt();
        
        boolean esPrimo = true;
        for (int i = 2; i <= Math.sqrt(numero); i++) {
            if (numero % i == 0) {
                esPrimo = false;
                break;
            }
        }
        
        if (numero < 2) {
            System.out.println("El número debe ser mayor o igual a 2.");
        } else if (esPrimo) {
            System.out.println("El número " + numero + " es primo.");
        } else {
            System.out.println("El número " + numero + " no es primo.");
        }
        
        scanner.close();
    }
}
