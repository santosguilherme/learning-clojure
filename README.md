# learning-clojure

## Clojure

Preparing the environment
https://clojure.org/guides/getting_started

## Aula 1 - Primeiras funções

> clojure.lang.IFn é uma indicação de que o código fonte de clojure é, pelo menos, parcialmente implementado em Java. No Github você pode encontrá-lo: https://github.com/clojure/clojure/.
Para quem já programa em Java, percebe alguns padrões: os desenvolvedores e desenvolvedoras de Clojure usaram o padrão I para definir uma interface e abreviaram Function para Fn, para condizer com o termo fn de Clojure ao invés do conceito de Function em si. Para quem quiser se aprofundar na implementação da linguagem, como uma função é invocável, esperamos que ela tenha um método a ser invocado, e olhando o código fonte dela encontramos o método invoke com suas n variações: https://github.com/clojure/clojure/blob/master/src/jvm/clojure/lang/IFn.java.

### O que aprendemos nesta aula:
- Mostrar uma mensagem na tela com o comando `println`;
- Que toda invocação de função colocamos parênteses entre ela;
- Definir uma variável global com `(def sua variavel )`;
- Criar um vetor `(def exemploVetor [“1”,”2”)`;
- Que para o Clojure a vírgula é considerada um espaço;
- Contar quantos elementos tem em um vetor com o `count`;
- Adicionar elementos ao vetor com o `conj`;
- Que o Clojure é imutável;
- Criar função com `defn`.

## Aula 2 - Símbolos e condicionais

> BigInt e BigDecimal não vão apresentar os tradicionais erros silenciosos de estouro em algumas linguagens, isto é, pegue o maior número de um Long e some 1, ele estoura. Pegue o menor Long possível e tire 1, ele estoura. Em Clojure, se o tipo de seu dado é Long ou Double ele automaticamente é passado para BigInt e BigDecimal, evitando tais situações, entre outros benefícios.

> Para ser um pouco mais formal, if é uma forma, não é uma função, e é uma forma especial https://clojure.org/reference/special_forms#if. Na prática, formas especiais podem ser utilizadas em nosso código e se misturam com as funções que invocamos em diversos momentos. Em geral, serão formas especiais aquelas que formam a base mínima da linguagem, uma maneira tradicional que as linguagens encontram para que a maior parte da mesma seja implementada na própria linguagem. Por exemplo, a função count é escrita na linguagem Clojure utilizando condicionais. Na prática, formas como if, let etc e funções aparecem misturadas em nosso código o tempo todo e por vício de linguagem é comum chamar uma forma especial de função, apesar da mesma ser uma forma.

### O que aprendemos nesta aula:
- Definir uma variável com `def` ela tem o escopo global, dependendo do namespace;
- Algumas boas práticas com Clojure;
- Criar uma variável de escopo local com o `let`;
- Utilizar o `class` para descobrir o tipo da variável;
- Trabalhar com condicionais `if`;
- Que o Nulo é considerado false dentro do `if`.

## Aula 3 - Funções anônimas e lambdas

https://github.com/alura-cursos/clojure-introducao/archive/aula2.zip

### Shortcuts:
- `cmd + shift + L` = load file in RPLF
- `cmd + shift + P` = executa código no contexto
- `cmd + shift + J` = poe para fora (barf)
- `cmd + shift + K` = poe para dentro (slurp)