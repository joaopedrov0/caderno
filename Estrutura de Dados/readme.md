# Eficiência

## Medição de Eficiência

### Medição por tempo

Mede eficiência do software com base no tempo que ele leva para executar a tarefa.

#### Problemas da medição por tempo

Apesar da precisão, alguns dos problemas medição por tempo de execução são a variação de resultados a depender do hardware em que está sendo executado, e a inviabilidade desse método em algoritmos que trabalham com uma quantidade muito grande de dados por conta do tempo que levaria para concluir.

### Medição por espaço

Mede eficiência do software com base na memória usada para executar a tarefa.

### Como escolher?

A escolha do método a ser utilizado para medir a eficiência depende do objetivo do sistema. Deve-se analisar qual é a prioridade do seu problema que o sistema deve resolver, se é trabalhar com recursos de memória mais escassos, ou dispor de um alto tempo de resposta.

## Medição por Contagem de Instruções



# Análise de Complexidade

## Perguntas da análise

- Ao dobrar o n, o n° de passos dobra? Ou então não muda? Ou vai além?
- Ao dobrar o n, a memória dobra? 
- O que é medir? Obter a ordem de grandeza da quantidade de passos executados de acordo com o tamanho da entrada


# Pesquisa

## Pesquisa Sequencial

A pesquisa ordenada consiste em uma pesquisa que passa por um vetor de modo sequencial, ou seja, partindo do início e percorrendo a lista até que encontre o que busca.

### Pesquisa Sequencial em Vetor Não-ordenado

A pesquisa sequencial quando feita em vetor não-ordenado passa por todos os elementos do vetor até encontrar o que procura, ou até o final caso não encontre o elemento que busca.

### Pesquisa Sequencial em Vetor Ordenado

No caso de uma pesquisa sequencial em um vetor ordenado, acontece algo semelhante porém tem uma diferença nos casos em que o elemento não está na lista.
Por exemplo, em uma lista ordenada, se o algoritmo estivesse procurando o número 7 e ele não estivesse na lista, ele saberia que poderia parar de procurar no momento em que encontrasse o número 8 mas não o 7.

## Pesquisa Binária

A pesquisa binária só existe para vetores ordenados e consiste na quebra do vetor na metade de forma recursiva até encontrar o elemento.
Por exemplo, observe o seguinte vetor:

```python
example = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

Se quiséssemos encontrar o elemento 7 nesse vetor, usando pesquisa binária seguiriamos as seguintes operações

- Pegaríamos o índice do meio (no caso o elemento 5 no índice 4)
- Verificamos se o elemento do meio é o que buscamos (No caso, não é)
- Verificamos se o elemento que buscamos é maior ou menor que o elemento do meio (Nesse caso 5 < 7)
- Pegamos a metade que contém o elemento que buscamos e em seguida repetimos o processo até encontrar

# Ordenação

Em breve...