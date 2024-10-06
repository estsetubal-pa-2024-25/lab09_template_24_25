# Programação Avançada | Lab9

:gb: [English version](README_EN.md)

## Objectivos
- Identificação de bad smells no código e respetivo refactoring
- Criação de testes unitários

## 1 - Introdução

O processo de *refactoring* é o processo de alterar um programa de *software*, através da melhoria da sua estrutura interna (desenho), sem alterar o seu comportamento. Este processo melhora o desenho do programa de *software*, torna o código mais eficiente, mais fácil de manter e – por conseguinte – facilita a compreensão do código, pois na maioria dos ambientes de desenvolvimento de *software*, outras pessoas que não desenvolveram o código terão que o ler.

Neste laboratório pretende-se que o aluno identifique os *bad smells* existentes no código e que aplique as devidas técnicas de *refactoring*, a fim de promover o desenvolvimento de código “limpo”. Aliando a literatura teórico-prática, sugere-se a leitura do conteúdo existente em https://refactoring.guru/refactoring/smells. Também poderá ser útil consultar a documentação do IntelliJ IDEA sobre as funcionalidade de *refactoring* disponibilizadas pelo IDE que poderão facilitar e acelerar algumas das operações a realizar: https://www.jetbrains.com/help/idea/refactoring-source-code.html

O projeto é baseado numa simples ferramenta de publicação de *reviews* sobre um dado produto. Ao utilizador é pedido somente para introduzir *reviews*, de modo a popular uma lista deste tipo.

![Figura 1 - Exemplo da interface gráfica](images/fig01.png)

Figura 1 - Exemplo da interface gráfica

## 2 - Exercícios

1. Nível 1: A classe **Review** apresenta um *bad smell* do tipo *data clump*.
   1. Identifique-o e faça o *refactoring* adequado para a resolução do problema;
   2. Confirme a correção da alteração anterior criando e executando um teste unitário adequado.
2. Nível 2: A classe **MainGUI** apresenta um *bad smell* do tipo *duplicate code*.
   1. Aplique a técnica *Extract Method* de forma a resolver o *duplicate code* encontrado no método *start*.
   
3. Nível 3: A classe **MainGUI** apresenta um *bad smell* do tipo *long method*.
   1. Aplique a técnica *Extract Method* de forma a resolver o *long method* no método *start* partindo-o em vários métodos.
4. Nível 4: A classe **Reviews** apresenta dois *bad smells*.
   1. Identifique-os e crie o teste unitário que valida o número total de reviews;
   2. Efetue o devido *refactoring* mencionando as técnicas utilizadas (sugestão para um deles: *Replace Inheritance with Delegation*);
   3. Confirme a correção da alteração anterior executando o teste unitário.
5. Nível 5
   1. Aplique a técnica *Extract Class*, de forma a extrair a responsabilidade da interface com o utilizador para uma classe denominada **GUIReviews**.

(fim de enunciado)