# potenciadedois

package potenciadedois;

import java.util.Scanner;

public class PotenciaDeDois {

   
    public static void main(String[] args) {
        
        
        Scanner scanner = new Scanner(System.in);

        // Solicita ao usuário que insira o número
        System.out.println("Digite um número inteiro positivo:");
        int numero = scanner.nextInt();

        // Verifica se o número é uma potência de dois
        boolean ehPotenciaDeDois = false;
        if (numero > 0 && (numero & (numero - 1)) == 0) {
            ehPotenciaDeDois = true;
        }

        // Exibe o resultado
        if (ehPotenciaDeDois) {
            System.out.println(numero + " é uma potência de dois.");
        } else {
            System.out.println(numero + " não é uma potência de dois.");
        }

        // Fecha o scanner
        scanner.close();
        
    }
    
}
