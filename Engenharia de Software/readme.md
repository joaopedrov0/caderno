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

Os membros da equipe trabalham ao mesmo tempo, não dependendo do progresso de outros processos para dar andamento no seu próprio.

## Técnicas de quarta geração

Engloba um conjunto de ferramentas de software que possibilitam que o sistema seja especificado em linguagem de alto nível e o código fonte seja gerado automaticamente a partir dessas especificações

Exemplo: Figma

Etapas:

- Obtenção de requisitos
- Estratégia de projeto
- Implementação usando técnicas de quarta geração
- Testes

## Métodos Formais

Especificar, desenvolver e verificar um sistema pela aplicação de uma notação matemática

Desenvolvimento do programa em modelo matemático, seguido de um cálculo de probabilidade de corretude do programa.

> Cleanroom: exemplo mais conhecido. Desenvolvimento incremental onde a correção de cada etapa é demonstrada com um experimento estatístico.

Como pontos negativos, esse método pode ser de difícil compreensão e corre o risco de ser um desperdício no desenvolvimento de sistemas simples e cotidianos.

Como pontos positivos, esse método é útil para sistemas que não podem falhar em hipótese alguma, onde caso contrário os resultados seriam catastróficos, portanto, é necessário ter 100% de certeza de que o sistema terá sucesso, e para isso é válido recorrer ao rigor matemático. Exemplos de sistemas críticos onde é válido usar esse método, seriam sistemas de controles de usinas nucleares, controle de tráfego aéreo e sistemas de UTIs.

## _Rapid Application Develpment_ (RAD)

Método que consiste na quebra do sistema em diferentes funcionalidades que serão distribuidas entre várias equipes que ficarão responsáveis por desenvolvê-las

Observe o exemplo abaixo

### Equipe 1

- Modelagem do negócio
- Modelagem dos dados
- Modelagem do processo
- Geração da aplicação (Componentes e técnicas de 4G - Quarta Geração, não confundir com 4g de dados móveis)
- Teste e modificação

### Equipe 2

- Modelagem do negócio
- Modelagem dos dados
- Modelagem do processo
- Geração da aplicação (Componentes e técnicas de 4G - Quarta Geração, não confundir com 4g de dados móveis)
- Teste e modificação

Trabalho paralelo entre as equipes

Como pontos positivos, esse método tende a resolver as funcionalidades com uma velocidade atraente

Como pontos negativos, naturalmente a divisão de pequenas funcionalidades em diferentes equipes vai requerer muitos profissionais para compor as equipes

## Métodos Ágeis

Voltados a softwares cujos requisitos são vagos ou mudam constantemente

- _Feature Driven Development_ (FDD)
- _Crystal Clear_
- _Dynamic Systems Development Method_ (DSDM)
- _eXtreme Programming_ (XP)

Características:

- Times pequenos e multidisciplinares
- Envolvimento do cliente
- Desenvolvimento iterativo e incremental
- Iterações curtas
- Desenvolvimento orientado a teste
- Quadro de tarefas
- Reunião diária
- Integração contínua (Não fazer a integração apenas no final do desenvolvimento)
- Programação em pares (Pair Programming)
- Refatoração do código (Revisar o código, se abrange todos os casos, organizar, etc.)
- Documentar apenas o necessário

Um possível problema desse método é a não disponibilidade do cliente para ter tanto contato com a equipe de desenvolvimento.

Técnicas que podem ser usadas em conjunto com outros modelos de processo vistos anteriormente.


## Processo Unificado

Baseado nos modelos incremental, espiral e de componentes

Tenta reunir os pontos positivos dos modelos apresentados anteriormente

Principais características:

- Baseado em casos de uso (Exemplos de uso, uma situação que pode acontecer no sistema)
- Iterativo e incremental 
- Centrado em arquitetura

Esse modelo baseia sua construção encima dos casos de uso que se espera do sistema.

Se apoia na arquitetura de interação entre os componentes

Composto por ciclos que são divididos em fases

Propôe um repositório de componentes, assim como no modelo de componentes.

> Níveis de abstração: Processo > Ciclos de desenvolvimento > Fase > Iteração

Fases do ciclo:

- Concepção
- Elaboração
- Construção
- Transição

Cada mudança de fase tem um **marco de referência**, cada mudança de iteração demarca uma versão diferente.

Iterações das fases são divididas em disciplinas

Disciplinas:

- Modelagem de Negócios
- Requisitos
- Análise e Design
- Implementação
- Teste
- Implatação
- Geren. de Configuração e Mudança
- Gerenciamento de Projeto
- Ambiente

Iterações das fases:

- Iniciação
- Elaboração
- Construção
- Transição

Artefatos (produtos gerados ao longo do desenvolvimento)

- Modelo de casos de uso
- Modelo de análise
- Modelo de projeto
- Modelo de implementação
- Modelo de implantação
- Modelo de testes
- Representação da arquitetura


