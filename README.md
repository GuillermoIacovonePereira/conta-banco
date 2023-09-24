# Simulando uma criação de uma Conta no Banco

~~~
import java.util.Scanner;

public class ContaTerminal {
    
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Por favor! Digite o numero da Conta, Agencia e seu Nome! ");
        int numeroConta = scanner.nextInt();

        String numeroAgencia = scanner.next();

        String nomeCliente = scanner.nextLine();
        nomeCliente = scanner.nextLine();
        
        System.out.println("\nOlá " + nomeCliente + ", obrigado por criar uma conta em nosso banco!\n Sua agência é: " + numeroAgencia + "\n Conta: " + numeroConta);

        System.out.println("Deseja ver o seu saldo atual? ");
        String resultadoSaldo = scanner.nextLine();

        if(resultadoSaldo.contains("Sim") || resultadoSaldo.contains("sim")){
            System.out.println("Saldo inexistente!");
        }else{
            System.out.println("Obrigado por usar o nosso banco!");
        }
        
    }
}
~~~
