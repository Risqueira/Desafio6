# Desafio6

# questao 1
```java
package tecnica.de.xiru;

/**
 *
 * @author henrique
 */
public class TecnicaDeXiru {

    public static void main(String[] args) {

        int numero;
        numero = 100;
        while (numero >= -100) {
            System.out.println(numero);
            numero--;
        }
    }

}
```
# questao 2
```java
package tecnica.de.xiru;

/**
 * Soma dos números pares: 2. Escreva um programa que calcule a soma dos números
 * pares de 1 a 20 utilizando um loop
 *
 * @author henrique
 */
public class TecnicaDeXiru {

    public static void main(String[] args) {

       int numero, soma;
        numero = 1;
        soma = 0;
        while (numero <= 20) {
            if (numero % 2 == 0) {

                soma += numero;
            }
            numero++;
        }
        System.out.println("a soma dos numeros pares:" + soma);

    }
}

````
# questao 3
```java
package tecnica.de.xiru;

import java.util.Scanner;

/**
 * Leitura de números até encontrar zero: 3. Escreva um programa que solicite
 * números ao usuário até que ele insira zero e, em seguida, exiba a soma dos
 * números digitados.
 *
 * @author henrique
 */
public class TecnicaDeXiru {

    public static void main(String[] args) {

        int numero, soma;
        Scanner ler = new Scanner(System.in);
        soma = 0;
        numero = 1;

        while (numero != 0) {
            System.out.println("Digite um numero:");
            numero = ler.nextInt();
            if (numero != 0) {
                soma += numero;
            }

        }
        System.out.println("A soma dos numeros é:" + soma);
    }
}
```
# questao 4
```java
package tecnica.de.xiru;

import java.util.Scanner;

/**
 * 4. Escreva um programa que calcule o fatorial de um número fornecido pelo
 * usuário usando um loop do-while.
 *
 * @author henrique
 */
public class TecnicaDeXiru {

    public static void main(String[] args) {

        Scanner ler = new Scanner(System.in);
        int numero, cont, i;
        cont = 1;
        i = 1;

        System.out.println("Digite um número:");
        numero = ler.nextInt();
        if (numero < 0) {
            System.out.println("Número invalido");

        }

        do {
            cont *= i;
            i++;
        } while (i <= numero);

        System.out.println("o fatorial do " + numero + " digitado é:" + cont);
    }
}
```
# questao 5
```java
package javaloop;

import java.util.Scanner;

/**
 * Jogo de adivinhação: 5. Escreva um programa que implemente um jogo de
 * adivinhação onde o usuário deve adivinhar um número entre 1 e 100, utilizando
 * um loop do-while para repetir até que o usuário acerte o número. O numero da
 * sorte deverá ser randomizado pelo computador, pesquise como funciona a
 * biblioteca Math.random()
 *
 * @author Henrique
 */
public class JavaLoop {

    public static void main(String[] args) {
        int nSorte, n;
        boolean achou;
        Scanner ler = new Scanner(System.in);
        achou = false;

        //Para nao dá loop no Math.random
        nSorte = 1 + (int) (Math.random() * 100);
        do {
            System.out.println("Digite seu numero da sorte de 1 a 100:");
            n = ler.nextInt();
            if (n == nSorte) {
                System.out.println("VOCÊ ACERTOU-PARABENS");
                achou = true;
            } else {
                System.out.println("ERROU XIRU!");
                System.out.println(nSorte);
            }
        } while (!achou);
        //enquanto ele for verdadeiro ele mantem o loop ate achar

    }

}
```
# questao 6
```java
package javaloop;

import java.util.Scanner;

/**
 * Tabuada de multiplicação: 6. Escreva um programa que exiba a tabuada de
 * multiplicação de um número fornecido pelo usuário usando um loop for. Você
 * deve informar o numero e de quanto a quanto você quer fazer a tabuada por
 * exemplo: tabuada do 2 de 1 a 20.
 *
 * @author Henrique
 */
public class JavaLoop {

    public static void main(String[] args) {
        int n, inicio, fim, i;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite um numero:");
        n = ler.nextInt();
        System.out.println("Digite o inicio da tabuada:");
        inicio = ler.nextInt();
        System.out.println("Digite o fim da tabuada");
        fim = ler.nextInt();

        if (inicio >= fim) {
            System.out.println("O inicio da tabuada não deve ser maior ou igual");
        } else {
            System.out.println("Tabuado do " + n + " de " + inicio + " ate " + fim + ":");
            for (i = inicio; i <= fim; i++) {
                System.out.println(n + " x " + i + " = " + (n * i));
            }
        }
    }

}
```
# questao 7
```java
package javaloop;

/**
 * Soma dos números ímpares: 7. Escreva um programa que calcule a soma dos
 * números ímpares de 1 a 200 utilizando um loop for.
 *
 * @author Henrique
 */
public class JavaLoop {

    public static void main(String[] args) {
        int n, soma;
        n = 1;
        soma = 0;

        for (n = 1; n <= 200; n++) {
            if (n % 2 != 0) {
                soma += n;
            }
        }
        System.out.println("A soma dos numeros impares de 1 a 200:" + soma);

    }

}

```
