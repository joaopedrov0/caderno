# Teoria Geral de Sistemas


## O que é um sistema?

Um conjunto de partes que trabalham juntas para atingir um objetivo em comum. Como por exemplo o corpo humano, formado por várias partes que trabalham juntas para manter o indivíduo vivo

## O que é um sistema complexo?

Um sistema complexo é um sistema no qual seu escopo e propriedades não são consequências diretas de cada parte que o compõe diretamente. O sistema complexo tem parte de suas propriedades emergêntes do que surge exclusivamente da interação das partes, e não apenas a soma das propriedades das partes que o forma.

Por exemplo, uma caneca de café com leite não tem gosto nem de café, nem de leite, a mistura das duas bebidas gera uma nova propriedade que não existia em nenhuma das partes que o compõe, mas a interação entre elas gerou essa propriedade nova.

### Sistemas complexos são "não-lineares"

Um sistema complexo se retroalimenta durante o funcionamento, interagindo consigo mesmo e, consequentemente, fazendo com que um sistema complexo não necessáriamente apresente sempre a mesma saída para uma determinada entrada.

> Na grande maioria das vezes, as pessoas podem acabar usando o sistema de uma forma diferente da que você idealizou quando criou o software, portanto é importante ter isso em mente durante a construção do programa.

## Importância das partes do desenvolvimento de um sistema

### Hardware



### Software



### Documento



### Pessoas

Entender o público alvo e as pessoas envolvidas no desenvolvimento


## Relação entre mudanças e índices de falha

Mudanças em um sistemas adicionam novas funcionalidades, se adaptando melhor às funcionalidades do público alvo se distanciando da obsolecência, mas também aumentam o índice de falhas.

# Processo de Software

## Definição

- Planejamento do projeto
- Levantamento de Requisitos
- Análise do sistema

Planejamento e conversa com o cliente para acertar qual o objetivo do sistema e quais devem ser as funções a serem cumpridas por ele e confirmação com o cliente de que o planejamento do projeto condiz com o que ele quer.

## Construção

- Projeto do sistema
- Codificação
- Teste

Etapa de esquematização técnica do sistema, codificação e testes para garantir que qualquer entrada não será capaz de quebrar o sistema.

## Manutenção

- Correção
- Adaptação
- Melhoria
- Incremento

Atividades realizadas após a entrega do sistema, são pequenas melhorias na interface ou funcionalidades que podem ser realizadas depois que o sistema já está entregue.

## Atividades de apoio

- Gerenciamento de configuração
- Garantia de qualidade
- Acompanhamento e controle

Orientações que podem servir de auxílio durante todos os três processos anteriormente mencionados. Acompanhamento de cronograma.

> O foco da disciplina está mais no levantamento de requisitos, análise, projeto do sistema e codificação. A grosso modo, o foco é conseguir esquematizar o sistema e, posteriormente, transformá-lo em código.

# Modelos de processo de software

## Modelo Cascata

"Ciclo de vida clássico"

"Modelo sequencial linear"

Etapas:
- Levantamento de requisitos
- Análise
- Projeto
- Codificação
- Teste
- Manutenção

A cada etapa que se passa nesse método, não se volta mais atrás. Por exemplo, uma vez que se finaliza o projeto, nunca mais haverá uma alteração no projeto.

Esse modelo tem a desvantagem de não ter planos para imprevistos e, caso algum problema ocorra em uma etapa passada, ele permanecerá lá.

Como vantagem, ele é um modelo simples de entender e bem organizado. Além de ser claro de determinar o que está sendo feito, como só se faz aquilo determinado na etapa atual, supõe-se que será bem feito.

## Modelo de Prototipação

As atividades se repetem iterativamente.

Criação de protótipos cada vez mais refinado

Etapas:
- Obter requisitos
- Elaborar projeto rápido
- Construir protótipo
- Avaliar protótipo **se estiver no ponto ideal, seguir adiante, caso contrário, retornar à etapa inicial**
- Usar protótipo como modelo para construir sistema com qualidade

Como problema desse modelo, pode ser que o protótipo seja usado como sistema final. Além disso, nesse modelo o processo acaba levando um tempo imprevisível, requerindo um estabelecimento de limite de refinamento do protótipo. Também tem o problema de o cliente ver o protótipo e ter a falsa impressão de que já está pronto para uso, pressionando a equipe a entregá-lo prematuramente pela urgência da solução do problema que o sistema deve resolver.

## Modelos evolutivos

### Incremental

Modelo iterativo que foca em entregar um produto operacional em cada incremento.

Modelo baseado na criação de pequenos pedaços do sistema, porém bem trabalhados para que essa parte pequena já fique pronta e funcional.

Etapas:
> Primeiro pedaço
- Análise **Primeiro pedaço do projeto**
- Projeto (design) **Primeiro pedaço do projeto**
- Codificação **Primeiro pedaço do projeto**
- Teste **Primeiro pedaço do projeto**
- **Entrega do primeiro incremento**
> Segundo pedaço
- Análise **Segundo pedaço do projeto** Considerando os problemas encontrados no incremento anterior
- Projeto (design) **Segundo pedaço do projeto** Considerando os problemas encontrados no incremento anterior
- Codificação **Segundo pedaço do projeto**
- Teste **Segundo pedaço do projeto**
- **Entrega do segundo incremento**
> Terceiro pedaço
- Análise **Terceiro pedaço do projeto** Considerando os problemas encontrados no incremento anterior
- Projeto (design) **Terceiro pedaço do projeto** Considerando os problemas encontrados no incremento anterior
- Codificação **Terceiro pedaço do projeto**
- Teste **Terceiro pedaço do projeto**
- **Entrega do terceiro incremento**

> Observação: Existem alguns sistemas onde a funcionalidade deles está no todo, não fazendo sentido realizar pequenas entregas de funcionalidades isoladas.

Como pontos positivos, o contato com o cliente é maior, tendo mais comunicação e a sensação de andamento do projeto.

Como pontos negativos, sistemas em que a funcionalidade principal está no todo tem suas pequenas funcionalidades isoladas inutilizadas.

### Espiral

Dividido em regiões de tarefas. Cada região possui um conjunto de tarefas, que são adaptadas às características de cada projeto.

Modelo organizado em ciclos

Exemplo de possiveis etapas:
#### Ciclo de Requisitos
- Planejamento (Planejamento dos requisitos)
- Análise de Risco (dos requisitos)
- Construção (dos requisitos)
- Avaliação (Avaliação dos requisitos. Mostrar ao cliente e verificar se é isso que ele quer)
#### Ciclo de Protótipo
- Planejamento
- Análise de Risco
- Construção
- Avaliação
#### Ciclo de Implementação
- Planejamento
- Análise de Risco
- Construção
- Avaliação

### Desenvolvimento Baseado em Componentes

Compõe aplicações a partir de componentes de software "empacotados".

Etapas de codificação:
- Identificar componentes candidatos
- Procurar componentes na biblioteca
- Extrair componente se disponível OU Construir componentes se indisponível e incluí-lo na biblioteca
- Construir n° iteração do sistema

Note que esse modelo pode ser um problema para uma empresa que está apenas começando a usar componentes, uma vez que ela inicialmente não tem nenhum componente na bibliteca

### Desenvolvimento Concorrente

Considera que membros do projeto levam seus processos ao mesmo tempo em fases diferentes do desenvolvimento cada processo estando em um estado diferente.

Etapas:

Etapas do engenheiro de software:

- Diagrama de classes
- Diagrama de sequência
- Modelo lógico do banco

Etapas do programador:

- Preparação do ambiente
- Implementação das classes
- Implementação dos métodos

## Cascata

## Cascata

## Cascata

## Cascata

## Cascata

## Cascata

