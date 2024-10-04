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

Nesta seção vamos estudar alguns algoritmos de Ordenação, úteis para, por exemplo, viabilizar a **Pesquisa Binária**.

Vale ressaltar que você pode usar estes algoritmos com qualquer lista que conhenha qualquer tipo de dado que você seja capaz de estabelecer uma ordem de alguma forma. Apesar disso, para fins didáticos e de facilitar o entendimento de cada algoritmo, foi utilizado números e na ordem crescente.

Outro detalhe importante é que os algoritmos de ordenação trabalham bastante com as comparações de maior e menor, o que já funciona perfeitamente para números. Caso você queira ordenar outro tipo de dado, como uma string, pode usar a ordem alfabética para isso, ou então alguma tabela como unicode ou ASCII dependendo no que você estiver trabalhando.

Também vale dizer que aqui não vai ter código de fato em nenhuma linguagem, apenas uma sintaxe genérica para representação de listas, escolhi fazer dessa forma pois o objetivo não é dar o passo a passo de como fazer cada tipo de algoritmo de ordenação, e sim fazer você entender a lógica por trás deles, pra aí sim você poder pensar em como implementar ele com a ferramenta e dados que você tiver em mãos.

## Selection Sort (Ordenação por Seleção)

No *Selection Sort*, é feita uma ordenação com base na busca do primeiro ou último termo de uma lista. A ideia é que, posição a posição, você identifique qual elemento deve estar ali.

Por exemplo, considere que você tenha uma lista de 10 números, do 1 ao 10 de modo desordenado, e queira ordena-la de modo crescente. Nesse caso, você vai procurar pelo menor número da lista (no nosso caso, o número 1) e trocá-lo de posição com o primeiro item da lista.

Depois de posicionado o primeiro elemento da forma correta, você parte então para a segunda posição, e procura na lista, considerando do segundo elemento pra frente apenas, qual o menor elemento daquela lista (no nosso caso, o número 2).

Para deixar mais claro como isso acontece, considere que a lista hipotética mencionada anteriormente seja essa aqui:

`[2, 3, 10, 9, 8, 4, 1, 5, 7, 6]`

Quando identificarmos que o primeiro elemento deve ser o 1 (pois estamos ordenando de forma **crescente** e o menor número da lista é o 1), podemos trocar ele de lugar com o atual primeiro elemento da lista, dessa forma:

`[1, 3, 10, 9, 8, 4, 2, 5, 7, 6]`

Sucessivamente, vamos continuar fazendo isso até que a lista inteira esteja ordenada:

Procurando o segundo termo:

`[1, 2, 10, 9, 8, 4, 3, 5, 7, 6]`

Procurando o terceiro termo:

`[1, 2, 3, 9, 8, 4, 10, 5, 7, 6]`

Procurando o quarto termo:

`[1, 2, 3, 4, 8, 9, 10, 5, 7, 6]`

Procurando o quinto termo:

`[1, 2, 3, 4, 5, 9, 10, 8, 7, 6]`

Procurando o sexto termo:

`[1, 2, 3, 4, 5, 6, 10, 8, 7, 9]`

Procurando o sétimo termo:

`[1, 2, 3, 4, 5, 6, 7, 8, 10, 9]`

Note que agora estamos procurando pelo oitavo elemento da lista, porém ele já está no seu devido lugar. Caso isso não tenha ficado claro, o que acontecerá aqui será que ele vai permanecer no mesmo lugar. Seria tipo trocar de posição com a exata posição em que ele está, entende? Por isso ele se mantém na posição correta

Procurando o oitavo termo:

`[1, 2, 3, 4, 5, 6, 7, 8, 10, 9]`

> Sim, durante essa iteração do nosso algoritmo, a lista permanecerá igual.

Procurando o nono termo:

`[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`

Por fim, invertidas as últimas duas posições, temos a lista devidamente ordenada, de modo crescente.

## Insertion Sort (Ordenação por Inserção)

A *Insertion Sort* busca partir de uma lista menor, e ir inserindo os novos elementos na sua posição correta, já de forma ordenada.

Por exemplo, observe a seguinte lista que queremos ordenar de forma crescente:

`[3, 5, 2, 5, 9, 7, 8]`

Nesse caso, podemos olhar para os dois primeiros elementos e notar que eles já estão ordenados de forma crescente, portanto, não precisamos mexer neles.

Lista atual: `[3, 5]`

Agora, vamos **inserir** o próximo elemento já na sua posição correta. No caso nosso elemento é o 2

Começando ali pelo 5, podemos comparar com o 2 e concluir que o 5 é maior que o 2, portanto, o 2 deve vir antes.

Comparando agora com o próximo elemento, concluímos que 3 também é maior que 2, portanto, nosso novo elemento acabou sendo inserido no início da nossa lista.

Lista atual: `[2, 3, 5]`

Agora, vamos adicionar o 5 à nossa nova lista ordenada.

Como 5 não é maior do que 5, já encontramos a posição ideal para ele. (Aqui no caso estamos verificando se o elemento novo é **maior** que o atual, mas se você fizer o contrário, e na hora de verificar, checar se ele é **menor**, você chegaria na mesma resposta, a diferença é que ele perceberia que 5 não é menor que 5, e passaria pra próxima comparação, quando ele percebesse que o número é menor do que 5, aí sim ele iria inserir na nova lista.)

Lista atual: `[2, 3, 5, 5]`

A partir daqui é só seguir nesse mesmo processo até chegar no final da lista e nossa nova lista ter a mesma quantidade de elementos que a original.

## Bubble Sort (Ordenação por Bolha)

O *Bubble Sort* consiste em basicamente percorrer uma lista analizando em pares os elementos consecutivos e invertendo-os de posição caso estejam em ordem errada, e repetir o processo até que toda a lista esteja ordenada.

Do ponto de vista de quem vai desenvolver o algoritmo, basicamente se cria um laço de repetição que vai analizar os elementos `lista[i]` e `lista[i+1]` e invertê-los caso necessário (Por exemplo, em uma ordem crescente, você inverteria os elemntos se `lista[i]` fosse maior que `lista[i+1]`)

## Merge Sort (Ordenação por Mesclagem)

O *Merge Sort* divide a lista e as sublistas resultantes ao meio até que cada parte tenha apenas 1 elemento. Depois disso, essas sublistas são mescladas aos poucos de forma ordenada até voltar ao tamanho da lista original

| lista[0] | lista[1] | lista[2] | lista[3] | lista[4] | lista[5] | lista[6] | lista[7] |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 5 | 6 | 3 | 1 | 4 | 8 | 7 | 2 |

Esta lista será dividida em 2, e as listas resultantes também, até que reste apenas 1 elemento por lista.

Nesse caso, nós vamos ter 3 "graus" de sublistas, ou seja, vamos dividir ao meio 3 vezes até que tenha apenas 1 elemento por lista.

| 1° Sublista de Grau 3 | 2° Sublista de Grau 3 | 3° Sublista de Grau 3 | 4° Sublista de Grau 3 | 5° Sublista de Grau 3 | 6° Sublista de Grau 3 | 7° Sublista de Grau 3 | 8° Sublista de Grau 3 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| `[5]` | ``[6]`` | ``[3]`` | ``[1]`` | ``[4]`` | ``[8]`` | ``[7]`` | ``[2]`` |

No momento de mergear (mesclar) as sublistas de grau 3, vamos adicioná-las às sublistas de grau 2 de modo ordenado, assim teremos estas 4 sublistas de grau 2:

| 1° Sublista de Grau 2 | 2° Sublista de Grau 2 | 3° Sublista de Grau 2 | 4° Sublista de Grau 2 |
| :---: | :---: | :---: | :---: |
| `[5, 6]` | `[1, 3]` | `[4, 8]` | `[2, 7]` |

> Observação: O termo "grau" de sublista não é algo que realmente existe, estou usando esse termo só para fins de explicação, eu criei esse conceito para facilitar o entendimento.

Depois disso, vamos mesclar essas sublistas resultantes, também de forma ordenada:

| 1° Sublista de Grau 1 | 2° Sublista de Grau 1 |
| :---: | :---: |
| `[1, 3, 5, 6]` | `[2, 4, 7, 8]` |

Por fim, vamos mesclar essas últimas duas sublistas e ter novamente uma lista com o tamanho original, 8 elementos.

| Lista Ordenada |
| :---: |
| `[1, 2, 3, 4, 5, 6, 7, 8]` |

## Quick Sort (Ordenação Rápida)

Semelhante a *Merge Sort*, a *Quick Sort* também usa uma divisão "ao meio" das listas e sublistas porém a diferença é que na ordenação rápida escolhe-se um pivô e posiciona-o no "centro" de uma nova lista onde os itens que devem vir antes dele são posicionados antes, e os que deveriam vir depois, são posicionados depois.

Por exemplo, vamos supor que precisemos ordenar uma lista desordenada com números de 1 a 10. Nesse método, se nosso pivô for 5 e nós quisermos ordenar a lista de modo crescente, todos os valores menores que cinco deverão vir antes do 5, e os elementos maiores, depois.

Note que não há necessidade de ordenar os elementos durante essa nova posição deles, pois depois de feita essa divisão e redisposição dos elementos, um novo pivô será escolhido para cada sublista e esse processo se repetirá recursivamente até que sobre apenas 1 elemento em cada sublista, nesse caso, já estariam ordenados corretamente.

