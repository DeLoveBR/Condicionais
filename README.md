# 🎓 Sistema de Média de Notas em Java

Este projeto consiste em um programa em Java desenvolvido para praticar **estruturas condicionais encadeadas** e entrada de dados dinâmicas. O algoritmo calcula a média aritmética de três notas e define a situação final do aluno baseado em regras de corte.

## 📋 Cenário do Problema

O objetivo do programa é capturar notas escolares através do console e aplicar as seguintes regras de negócio baseadas na média final (**M**):
* **Média ≥ 9.0:** Aluno excelente. Exibe a mensagem `"Aprovado Parabens!!!"`.
* **Média entre 5.0 e 8.99:** Aluno mediano. Exibe a mensagem `"Ficou na Medeia"`.
* **Média < 5.0:** Aluno abaixo do esperado. Exibe a mensagem `" Recuperação"`.

---

## 💻 Código Fonte

Abaixo está o código fonte completo e estruturado dentro de sua classe principal, incluindo a importação necessária do pacote `java.util.Scanner`.

```java
import java.util.Scanner;

public class CalculoMedia {
    public static void main(String[] args) {
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
        float M = (nota1 + nota2 + nota3) / 3;

        // Exibe a média calculada
        System.out.println("A Média da sua nota é: " + M);

        // Verifica a situação do aluno de acordo com a média
        if (M >= 9) {
            // Média igual ou superior a 9: aluno aprovado com excelência
            System.out.println("Aprovado Parabens!!!");
        } else if (M >= 5) {
            // Média entre 5 e 8.99: aluno ficou na média
            System.out.println("Ficou na Medeia");
        } else {
            // Média inferior a 5: aluno em recuperação
            System.out.println(" Recuperação");
        }

        // Fecha o scanner para evitar vazamento de memória
        sc.close();
    }
}
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Você precisará do [JDK (Java Development Kit)](https://oracle.com) instalado na sua máquina (versão 8 ou superior).

### Passo a Passo

1. **Crie o arquivo:** Salve o código acima em um arquivo chamado `CalculoMedia.java`.
2. **Abra o terminal:** Navegue até a pasta onde o arquivo foi salvo.
3. **Compile o código:**
   ```bash
   javac CalculoMedia.java
   ```
4. **Execute o programa:**
   ```bash
   java CalculoMedia
   ```

---

## 📝 Conceitos Praticados

* Interação com o usuário via terminal usando a classe `java.util.Scanner`.
* Manipulação de tipos primitivos de ponto flutuante de precisão simples (`float`).
* Operadores aritméticos de soma e divisão com precedência de parênteses `()`.
* Estruturas condicionais compostas e encadeadas (`if`, `else if` e `else`).
* Boa prática de fechamento de recursos com `sc.close()`.
