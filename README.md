# Atividades Básicas de Java

---

## Questões

1. **Imprimir "Hello World" no terminal**  
   (Objetivo: Aprender a usar o método `System.out.println()` para exibir mensagens.)

2. **Declarar variáveis dos tipos primitivos**  
   (Objetivo: Compreender a declaração e o uso de variáveis e a distinção entre tipos primitivos e não primitivos.)

3. **Realizar operações aritméticas básicas**  
   (Objetivo: Aprender a utilizar os operadores matemáticos: `+`, `-`, `*`, `/` e `%`.)

4. **Utilizar a estrutura condicional `if/else`**  
   (Objetivo: Entender como controlar o fluxo de execução do programa com decisões condicionais.)

5. **Implementar um loop `for` para iterar de 1 a 10**  
   (Objetivo: Aprender a estrutura de repetição `for` e o uso de contadores.)

6. **Implementar um loop `while` que imprima números de 1 a 5**  
   (Objetivo: Aprender a estrutura de repetição `while` e a forma de atualizar condições.)

7. **Criar um método que receba dois números e retorne a soma**  
   (Objetivo: Aprender a declarar e utilizar métodos, bem como o conceito de passagem de parâmetros e retorno de valores.)

8. **Trabalhar com arrays: declarar, inicializar e acessar elementos**  
   (Objetivo: Compreender a declaração e manipulação de arrays em Java.)

9. **Utilizar o loop `for-each` para percorrer um array**  
   (Objetivo: Aprender a usar o loop aprimorado para iterar de forma simples sobre coleções ou arrays.)

10. **Criar uma classe com atributos, construtor e método, instanciar um objeto e chamar o método**  
    (Objetivo: Introduzir conceitos de classes, objetos, construtores e encapsulamento.)

---

## Correções e Exemplos

### 1. Imprimir "Hello World" no terminal
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```
*Explicação:* O método `System.out.println()` envia a mensagem para o terminal.

---

### 2. Declarar variáveis dos tipos primitivos
```java
public class Main {
    public static void main(String[] args) {
        int numero = 10;
        double valor = 5.99;
        char letra = 'A';
        boolean status = true;
        
        System.out.println("Número: " + numero);
    }
}
```
*Explicação:* Aqui usamos variáveis dos tipos primitivos: `int`, `double`, `char` e `boolean`.

---

### 3. Realizar operações aritméticas básicas
```java
public class Main {
    public static void main(String[] args) {
        int a = 8, b = 3;
        System.out.println("Soma: " + (a + b));
        System.out.println("Subtração: " + (a - b));
        System.out.println("Multiplicação: " + (a * b));
        System.out.println("Divisão: " + (a / b));
        System.out.println("Módulo: " + (a % b));
    }
}
```
*Explicação:* Demonstra o uso de operadores aritméticos para realizar cálculos.

---

### 4. Utilizar a estrutura condicional `if/else`
```java
public class Main {
    public static void main(String[] args) {
        int numero = 5;
        if (numero > 0) {
            System.out.println("Número positivo");
        } else {
            System.out.println("Número não é positivo");
        }
    }
}
```
*Explicação:* O `if/else` permite executar diferentes blocos de código com base em uma condição.

---

### 5. Implementar um loop `for`
```java
public class Main {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            System.out.println("Número: " + i);
        }
    }
}
```
*Explicação:* O loop `for` utiliza um contador para repetir um bloco de código.

---

### 6. Implementar um loop `while`
```java
public class Main {
    public static void main(String[] args) {
        int i = 1;
        while (i <= 5) {
            System.out.println("Contagem: " + i);
            i++;
        }
    }
}
```
*Explicação:* O loop `while` repete o bloco de código enquanto a condição especificada for verdadeira.

---

### 7. Criar um método que retorne a soma de dois números
```java
public class Main {
    public static void main(String[] args) {
        int resultado = soma(7, 3);
        System.out.println("Soma: " + resultado);
    }
    
    public static int soma(int x, int y) {
        return x + y;
    }
}
```
*Explicação:* Este exemplo demonstra como definir um método (`soma`) que recebe parâmetros e retorna um valor.

---

### 8. Trabalhar com arrays
```java
public class Main {
    public static void main(String[] args) {
        int[] numeros = {1, 2, 3, 4, 5};
        System.out.println("Primeiro número: " + numeros[0]);
    }
}
```
*Explicação:* Mostra a declaração, inicialização e acesso a elementos de um array.

---

### 9. Utilizar o loop `for-each`
```java
public class Main {
    public static void main(String[] args) {
        int[] numeros = {10, 20, 30, 40, 50};
        for (int num : numeros) {
            System.out.println("Valor: " + num);
        }
    }
}
```
*Explicação:* O loop for-each permite iterar de forma simples sobre todos os elementos de um array.

---

### 10. Criar uma classe com atributos, construtor e método
```java
// Definição da classe Pessoa
public class Pessoa {
    String nome;
    int idade;
    
    // Construtor
    public Pessoa(String nome, int idade) {
        this.nome = nome;
        this.idade = idade;
    }
    
    // Método para mostrar informações
    public void mostrarInfo() {
        System.out.println("Nome: " + this.nome + ", Idade: " + this.idade);
    }
}

// Classe principal
public class Main {
    public static void main(String[] args) {
        Pessoa pessoa = new Pessoa("Maria", 25);
        pessoa.mostrarInfo();
    }
}
```
*Explicação:* Este exemplo ensina como criar uma classe, definir atributos, implementar um construtor e um método, além de instanciar um objeto e utilizá-lo.

---

## Nova Parte da Sintaxe: Introdução à Orientação a Objetos (POO) em Java

A partir da atividade 10, iniciamos a introdução à Programação Orientada a Objetos (POO), que é fundamental para a construção de programas em Java. Aqui estão os conceitos básicos:

- **Classe:** Um molde que define propriedades (atributos) e comportamentos (métodos) dos objetos.
- **Objeto:** Uma instância de uma classe. É através dele que acessamos os atributos e métodos definidos na classe.
- **Construtor:** Um método especial usado para inicializar os atributos do objeto no momento em que ele é criado.
- **Encapsulamento:** A prática de proteger os dados dos objetos, permitindo acesso controlado através de métodos (getters/setters).

### Exemplo Completo com Orientação a Objetos
```java
// Definição da classe Carro
public class Carro {
    private String modelo;
    private int ano;
    
    // Construtor
    public Carro(String modelo, int ano) {
        this.modelo = modelo;
        this.ano = ano;
    }
    
    // Método para exibir informações do carro
    public void exibirInfo() {
        System.out.println("Modelo: " + modelo + " - Ano: " + ano);
    }
    
    // Método principal para testar a classe
    public static void main(String[] args) {
        Carro meuCarro = new Carro("Toyota", 2020);
        meuCarro.exibirInfo();
    }
}
```
*Explicação:*  
- **Classe `Carro`:** Define os atributos `modelo` e `ano` como privados para reforçar o encapsulamento.  
- **Construtor:** Inicializa os atributos quando um novo objeto `Carro` é criado.  
- **Método `exibirInfo()`:** Exibe as informações do carro no terminal.  
- **Método `main`:** Cria uma instância de `Carro` e chama o método para exibir seus dados.
