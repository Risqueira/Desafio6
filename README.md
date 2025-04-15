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
