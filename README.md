import java.util.Scanner;

public class Condicionais {
    public static void main(String[] args) {

        // Sistema de Média de Notas
        // Exercício desenvolvido para praticar estruturas condicionais em Java.

        // Cria o objeto Scanner para receber os dados digitados pelo usuário
        Scanner sc = new Scanner(System.in);

        // Solicita e recebe a primeira nota
        System.out.println("Digite sua primeira nota: ");
        float nota1 = sc.nextFloat();

        // Solicita e recebe a segunda nota
        System.out.println("Digite sua segunda nota: ");
        float nota2 = sc.nextFloat();

        // Solicita e recebe a terceira nota
        System.out.println("Digite sua terceira nota: ");
        float nota3 = sc.nextFloat();

        // Calcula a média das três notas
        float M = (nota1 +nota2 +nota3) /3;

        // Exibe a média calculada
        System.out.println("A Média da sua nota é: " +M );

        // Verifica a situação do aluno de acordo com a média
        if (M>=9){

            // Média igual ou superior a 9: aluno aprovado
            System.out.println("Aprovado Parabens!!!");

            // Média entre 5 e 8,99: aluno ficou na média
        } else if (M>=5) {
            System.out.println("Ficou na Medeia");

            // Média inferior a 4,99: aluno em recuperação
        }
        else {
            System.out.println(" Recuperação");
        }
    }
}
