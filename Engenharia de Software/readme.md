# Caderno de Engenharia de Software

Boas vindas ao caderno utilizado para tomar notas durante as aulas de Engenharia de Software I

# Sumário

[Teoria Geral de Sistemas](#teoria-geral-de-sistemas)

[Processo de Software](#processo-de-software)

[Modelos de Processo de Software](#modelos-de-processo-de-software)

[Gerenciamento de Configuração de Software](#gerenciamento-de-configuração-de-software)

[Levantamento de Requisitos](#levantamento-de-requisitos)

[Análise do Sistema](#análise-do-sistema)

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



# Gerenciamento de Configuração de Software

- Tarefas preliminares
- Identificação dos itens de configuração
- Controle de mudanças
- Controle de versão
- Auditoria de configuração
- Preparação de relatórios de estado
- Controle de interface
- Controle de subcontratados e fornecedores

## Configurações de software (Comparável à Versão de software)

Subconjunto de artefatos do desenvolvimento de software que terão suas alterações controladas

Exemplos de artefatos:

- Programas
- Diagramas
- Descrições de processos
- Manuais

## Marco de referência (Milestone)

Artefato que foi devidamente revisado e aprovado, portanto, confia-se que ele está correto e não se deve alterá-lo.

> Exemplo
> Ao final de uma Definição do Sistema, pode-se gerar um documento de Especificação do Sistema. Esse documento, quando devidamente revisado e aprovado, demarca o final da etapa de Definição do Sistema, portanto pode ser considerado um **Marco de Referência**.

Um Marco de Referência serve como base para construções futuras.

## Tarefas preliminares

### Seleção de itens a serem gerenciados

Uma documentação escassa pode não separar devidamente as tarefas a ponto de facilitar e organizar o desenvolvimento do projeto. Por outro lado, uma superdocumentação pode dividir demais, reduzindo os problemas a coisas extremamente simples, porém muito numerosas.

### Descrever como itens selecionados se relacionam

A identificação dos relacionamentos entre os itens é importnate para a manutenção. Permite que se localizem rapidamente os itens afetados em cada alteração.

### Planejar os referenciais dentro do ciclo de vida do projeto

Planejamento dos **Marcos de Referência**

### Descrever como os itens serão arquivados e recuperados do repositório

Definição de quem deve arquivar e recuperar itens no repositório e como isso deve ser feito.

## Identificação dos itens de configuração

Planejamento da identificação dos itens de configuração. Por exemplo, nomear um artefato com "vX.Y.Z" de acordo com sua versão dentro do planejamento to projeto. Estratégias de atribuição de nomes únicos também faz parte desta etapa.

Observe alguns exemplos de informações que podem ser reconhecidas pelo nome do item:

- Evolução de cada uma das versões dos componentes
- Hierarquia existente entre componentes
- Cliente
- Linguagem de programação
- Status do desenvolvimento
- Plataforma de hardware
- Data de criação

## Controle de mudanças

O controle de mudanças através de pedidos de alteração facilita a gerencia de quem faz o quê e quando. É possível, dessa forma, identificar tarefas mais importantes/urgentes.

Procedimentos formais de organização e de controle de mudanças no sistema permitem que:

- Os pedidos de alteração possam ser considerados em conjunto com outros pedidos
- Pedidos similares possam ser agrupados
- Pedidos incompatíveis, entre si ou com os objetivos do sistema, possam ser identificados
- Sejam atribuídas prioridades aos pedidos

> **slide 39 ????**

Exemplo de registro de solcitação de mudança:

- Projeto
- Responsável pela mudança
- Data da solicitação
- Mudança a ser feita
- Componentes afetados
- Justificativa
- Priotidade
- Tempo estimado
- Responsável pela autorização
- Data da autorização
- Autorização (Sim/Não)

## Controle de versões

Um item, ao ser desenvolvido, passa por vários estados, várias versões até que cumpra o propósito para o qual foi criado. Versões distintas podem incluir diversas alterações, como por exemplo:

- Funcionalidades distintas
- Desempenhos aprimorados
- Defeitos corrigidos
- Funcionalidades equivalentes, diferentes configurações de hardware e software

As versões são todas armazenadas e identificadas, mas com base nas alterações e não nos arquivos em si (por motivos óbvios de redução de custo de armazenamento), e para isso usam-se deltas

### Delta Negativo

Armazena as diferenças (deltas) existentes até então e a versão mais recente.

### Delta Positivo

Armazena a versão mais antiga e, para montas as vers~es mais recentes, processam-se as diferenças (deltas) armazenadas.

### *Release*

Uma liberação (ou *release*) é uma versão distribuída para os clientes. Naturalmente, é comum ter muito mais versões do que liberações.

## Auditoria de configuração

Assegura que as alterações foram implementadas apropriadamente

### Auditoria Funcional

Preocupa-se com aspectos internos dos arquivos, compreendendo uma verificação técnica formal dos itens de configuração (qualidade de software). Tenta descobrir omissões ou erros na configuração que degradam os padrões de construção do software.

### Auditoria Física

Processo administrativo que ocorre no final de cada fase do ciclo de vida do software.

Verifica a configuração a ser congelada como marco referencial

- Se é composta da versão mais recente dos itens de configuração
- Se os procedimentos e padrões foram devidamente aplicados

## Preparação de relatórios de estado

## Controle de Interface

## Controle de subcontratados e fornecedores


# Planejamento do Projeto

???


# Levantamento de Requisitos

Os requisitos são as condições que o sistema deve atender

Observe abaixo exemplos de tipos de requisitos importantes a serem definidos com exemplos entre parênteses:

- Requisito de Funcionalidade (Permitir que cada usuário tenha suas próprias configurações de fonte e imagem de fundo) `Requisitos Funcionais`
- Requisito de Restrição (Não permitir mais de 3 tentativas de autenticação dentro de 5 minutos) `Requisitos Funcionais`
- Requisito de Atributo de Qualidade (Efetivar pagamento em até 30 segundos) `Requisitos Arquiteturais`
- Requisito de Negócio (Direcionar o sistema para o público de 15 a 30 anos) `Requisitos Arquiteturais`

## Elicitação

Identificação dos Requisitos do sistema

### Análise de Domínio

Análise do ambiente em que o sistema será inserido

- Papéis, objetos, locais e eventos comuns
- Características e comportamentos recorrentes
- Palavras e jargões da área

> #### Exemplo no domínio de teatro
> - Ator, diretor, roteirista, palco, coxia, camarim, ensaio
> - Usar maquiagem e figurino, montar o cenário
> - *Performance*, "merda!"

Análises de Domínio podem ser feitas com interações com as partes interessadas no sistema (pessoas que têm algum interesse no sistema, *stakeholders*)

> #### Exemplos de *stakeholders*
> - Gerente de projeto (Gerenciamento de cronograma, orçamento)
> - Analista
> - Engenheiro de Software
> - Programador (Como por exemplo, alguma especificação técnica a respeito das ferramentas que seão utilizadas. "Não vamos usar a biblioteca X porque ela não está disponível para Linux")
> - Testador
> - Mantenedor
> - Cliente
> - Usuário (Funcionalidades)

> #### Exemplos de interações com as partes interessadas
> - Entrevistas
> - Questionários
> - Reuniões
> - Cenários (Descrição de uma interação com o sistema do ponto de vista de uma parte interessada)
> - Observação em campo
> - Estudo de dispositivos e sistemas de apoio
> - Estuod de documentos específicos
> - Consultoria especializada
> - Estudo de sistemas similares
> Exemplo de cenário: "Um usuário remoto solicita um relatório de um banco de dados pela internet durante um período de pico e recebe o relatório em cinco segundos."

## Especificação

Detalhamento dos requisitos

- Condição a ser atendida
- **Forma de medição e critério de satisfação (Métrica objetivamente testável)**
- Influência em e de outros requisitos
- Prioridade do critério adotado

| ID | Requisito | Forma de medição e critério de satisfação | Requisitos relacionados | Importância |
| --- | --- | --- | --- | --- |
| R4 | O sistema deve ser de fácio uso de forma que os usuários cometam poucos erros | Conta-se a média de erros que usuários escolhidos pelo cliente cometem no 1° mês de uso. O requisito é atendido se a média for de até 2 erros/dia | R1, R3 | Alta |

> Requisitos que exigem ou restringem funcionalidades para o usuário são chamados de requisitos funcionais

> Requisitos que definem atributos de qualidade ou de negócio são chamados de requisitos não funcionais, de qualidade ou arquiteturais

## Validação

Confirmação com as partes interessadas de que os requisitos especificados estão corretos e não está faltando nenhum.

Essa etapa é importante para detectar antecipadamente defeitos, aumentar a produtividade e diminuir o custo do projeto.

### Inspeção de Software

Leitura do doumento usando técnicas que dizem ao revisor o quê procurar no documento durante a leitura

- Leitura Baseada em Perspectiva (PBR)
- Lista de verificação (*checklist*)

#### Leitura Baseada em Perspectiva

A revisão é feita sob a perspectiva de cada parte interessada (cliente, usuário, gerente, programador, etc...). Caso não sera possível que todos os interessados revisem os requisitos, os membros do projeto devem assumir o papel desses interessados e fazem a revisão sob sua perspectiva.

#### Lista de verificação

Cria-se uma lista com questões quanto aos tipos de defeitos a se verificar nos requisitos e cada parte interessada percorre a lista de verificação conferindo a situação do sistema quanto a cada questão.

# Análise do Sistema

Definição do quê deve ser ser feito **para o cliente** validar.

Nesta etapa objetiva-se especificar o que o sistema deve fazer, e não como será feito.

Quando o cliente estiver de acordo com o que entendemos que o sistema deve fazer, aí sim devemos passar para as etapas de definir como isso deve ser feito.

Os documentos de comunicação com o cliente devem ser de alto nível de abstração, sem detalhes técnicos, facilitando ao máximo o entendimento do documento por leigos em computação.

Exemplos de documentos em alto nível de abstração

- Modelo de casos de uso
- Diagramas de sequência do sistema (um para cada caso de uso)
- Mapa de navegação
- Modelo conceitual
- Outros

## Casos de Uso

O modelo de casos de uso direciona diversas tarefas posteriores do ciclo de vida do software.

Além disso, o modelo de casos de uso força o desevolvedor a moldar o sistema de acordo com o usuário

O modelo de casos de uso modela os requisitos funcionais do sistema. Depende de que se tenha um entendimento ao menos parcial dos requisitos do sistema

Um modelo de casos de uso de um sistema compreende um diagrama de casos de uso e asa descrições desses casos

> ### Nota informal
> O modelo de casos de uso basicamente tentar se colocar no lugar do usuário final antes do sistema ser criado e imaginar como seria o uso do sistema, descrevendo ao máximo para ter um norte na hora do desenvolvimento

### Diagrama de Casos de Uso

É responsável por representar graficamente os atores, casos de uso, relacionamentos entre os elementos do sistema e seu limite.

- Casos de uso
- Atores
- Relacionamentos entre casos de uso e atores
- Limite ou Escopo do sistema

Tem o objetivo de ilustrar em um nível alto de abstração quais elementos **externos** interagem com quais **funcionalidades** do sistema.

#### O que são casos de uso?

Um caso de uso **representa quem faz o quê com o sistema, sem considerar o comportamento interno do sistema**.

> #### Nota informal
> Casos de uso são casos hipotéticos imaginários de uso do sistema.

O modelo de casos de uso é uma **representação das funcionalidades externamente observáveis do sistema** e dos elementos externos ao sistema que interagem com o mesmo.

> #### Nota informal
> Os casos de uso não se importam com o processo de uso de uma funcionalidade, mas sim com os pontos de interesse do sistema. Tipo, se tu fosse explicar pra algm oq q da pra fazer com Discord, tu n precisa falar nada de login nem nada do tipo, pode ir direto pra "fazer ligações" ou "organizar eventos" ou "gerenciar comunidades".


Um caso de uso é um **processo, relativamente grande, com início e fim próprios**, que  normalmente inclui várias transações ou operações de entrada e saída

Iniciado com verbo para enfatizar que é uma ação, como nos exemplos abaixo

- Sacar dinheiro (Caixa automático)
- Matricular-se em disciplina

Casos de uso **não** representam um passo individual ou uma operação interna. **Não** são casos de uso:

- Login
- Imprimir recibo

#### Atores

Elemento **externo** que **interage** com o sistema

- "Externo": atores não fazem parte do sistema
- "Interage": um ator troca informações com o sistema

Casos de uso representam uma sequência de interações entre o sistema e atores, no sentido de troca de inormações entre eles

Normalmente um agente externo inicia a sequência de interações com o sistema, ou um evento acontece para que o sistema responda.

Um ator corresponde a um **papel** representado em relação ao sistema

- Uma pessoa pode desempenhar o papel de Funcionário de uma instituição bancária que realiza a manutenção de um caixa eletrônico, mas também pode ser o Cliente do banco que realiza o saque de uma quantia.
- O mesmo indivíduo pode ser o Cliente que compra mercadorias e o Vendedor que processa vendas.

O nome dado a um ator deve lembrar o seu papel, ao invés de lembrar quem o representa

Exemplos de atores:

- Pessoas (Empregado, Cliente, Gerente, Almoxarife, Vendedor, etc.)
- Organizações (Empresa Fornecedora, Agência de Impostos, Administradora de Cartões, etc.)
- Outros sistemas (Sistema de Cobrança, Sistema de Estoque de Produtos, etc.)
- Equipamentos (Leitora de Código de Barras, Sensor, etc.)

O diagrama de casos de uso mostra o relacionamento entre os atores e os casos de uso dentro de um sistema

- Um caso de uso é representado por uma elipse contendo seu nome
- Um ator pode ser representado com um retângulo com o estereótipo `<<ator>>` ou pela figura de uma pessoa estilizada

> #### Nota Informal
> Um ator é literalmente qualquer coisa que interaja com o sistema de alguma forma e que n é vc que vai desenvolver, pode ser uma maquina, outro sistema, uma pessoa... qlq coisa.

#### Relacionamentos

Casos de uso e atores não existem sozinhos. Existem relacionamentos entre eles:

- Comunicação
- Inclusão
- Extensão
- Generalização ou Herança

##### Comunicação

- Representa a informação de quais atores estão associados a que casos de uso
- É o mais comum dos relacionamentos
- O fato de um ator estar associado a um caso de uso significa que esse ator interage (troca informações) com o sistema
- Um ator pode se relacionar com mais de um caso de uso

Um relacinamento de comunicação é representado por uma linha **sem ponta** ligando ator e caso de uso

Neste diagrama **não** se representa a ordem em que os casos de uso ocorrem

##### Inclusão

- Existe somente entre casos de uso
- A inclusão é representada por uma seta tracejada de ponta aberta do caso de uso base para o incluído com o estereótipo `<<inclui>>`
- Usado em dois casos
    1. Quando há funcionalidades distintas de interesse do usuário e, por coincidência, uma requer internamente a outra (Por exemplo, comprar um ingresso no cinema e verificar os lugares disponíveis. Não tem como comprar um ingresso sem verificar os lugares disponíveis, mas verificar os lugares disponíveis não requer a compra do ingresso, portanto, por ambas atividades por si só já são casos de uso válidos)
    2. Quando funcionalidades compartilham uma mesma sequência de passos para evitar repetição.
        Quando dois ou mais casos de uso incluem uma sequênia de interações em comum, esta sequência pode ser descrita em um outro caso de uso. Esse caso de uso em comum evita a descrição de uma mesma sequência de interações mais de uma vez e torna a descrição dos casos de uso mais simples

##### Extensão

- Existe somente entre casos de uso
- Utilizado para modelar situações onde diferentes sequências de interações podem ser inseridas em um caso de uso
- Cada uma das diferentes sequências representa um comportamento opcional, que só ocorre sob certas condições ou cuja realização depende da escolha do ator
- Separar um comportamento obrigatório de outro opcional
- Separar um trecho de casos de uso que será executado apenas em determinadas condições
- Separar trechos que dependam da interação com um determinado ator
- Um caso d euso estende outro se ele (eventualmente) adiciona comportaments ao caso de uso base
- Sejam A e B dois casos de uso
    - Um relacionamento de extensão de B para A indica que um ou mais dos cenários de A podem incluir o comportamento especificado por B
    - Neste caso, diz-se que B estende A
    - O caso de uso A é chamado de estendido e o caso de uso B o extensor
- Quando um ator opta por executar a sequência de interações definida no extensor, este é executado
- Após a sua execução, o fluxo de interações volta ao caso de uso estendido, recomeçando logo após o ponto em que o extensor foi inserido
- Não necessariamente o comportamento definido pelo caso de uso extensor é realizado
- Os relacionamentos de extensão são representados por uma seta tracejada de um caso de uso para outro. A seta recebe o estereótipo `<<estende>>` ou ``<<extends>>``.

##### Generalização ou Herança

A generalização (ou herança) acontece quando um ator ou caso de uso herda características de outro.

Imagine um sistema de gerenciamento de uma loja.

Nesse sistema existe um usuário que pode ter dois tipos diferentes, administrador e funcionário. Ambos fazem tudo que um usuário comum faz e mais algumas coisas específicas.

Até agora, temos os atores "Administrador" e " Usuário" que tem uma herança em comum, o ator "usuário"

Agora vamos para os casos de uso.

Imagine que dentro do sistema nós temos 3 casos de uso (apenas para fins didáticos).

- Gerenciar Dados
- Gerenciar Clientes
- Gerenciar Produtos

Nesse exemplo, Gerenciar Dados é um uso abrangente que engloba tanto o gerenciamento de clientes quanto o de produtos. Isso significa que o "Gerenciar de Clientes" e o "Gerenciamento de Produtos" estão contidos em "Gerenciar Dados", ou seja, tudo que "Gerenciar Clientes" faz, "Gerenciar Dados" também faz, e o mesmo ocorre com "Gerenciar Produtos".

Adicionalmente, podemos aprofundar mais ainda o exemplo, pois "Gerenciar Cliente" pode ter outros Casos de Uso que **herdam suas características**, como os exemplos abaixo:

- Excluir Cliente
- Adicionar Cliente
- Editar Cliente

Todos esses casos de uso hipotéticos teriam uma herança em comum, "Gerenciar Cliente", e todas as suas características estariam presentes nesse caso mais abrangente.

### Descrição Textual de Casos de Uso

A Descrição Textual de Casos de Uso se dá por meio de uma descrição "narrativa" de um exemplo de caso de uso, quase como uma "pequena história" mesmo. Elas contam o passo a passo de um ator em uma interação com o sistema.

#### Formas de caracterizar os Casos de Uso

- Formato
- Tipo
- Grau de detalhamento

##### Formato

- Descrição contínua
- Descrição numerada
- Descrição particionada

> ###### Nota Informal
> A descrição contínua é basicamente um texto em prosa descrevendo a interação entre o ator e o sistema, naturalmente organizado em parágrafos, etc.
> A descrição numerada meio que lista as interações entre o ator e o sistema de modo ordenado, numerado
> A descrição particionada é igual a numerada, com a diferença que ela divide as interações onde o ator age e onde o sistema age

##### Tipo

- Primários
    - Processos mais importantes
- Secundários
    - Processos menos importantes ou raros
- Opcionais
    - Processos que podem não ser incluídos no sistema


##### Grau de Detalhamento

- Alto nível ou Resumido
- Expandido ou Completo

Descrições em **Alto nível (ou Resumido)** descrevem o processo sucintamente, em duas ou três sentenças. São vagos a respeito de decisões de projeto e são úteis na fase inicial da engenharia de requisitos. Deve usar nome de atores com letra maiúscula e usar verbos para nomear os casos de uso.

Observe um exemplo em **Alto nível (ou Resumido)**

| Caso de uso | Resumo |
| --- | --- |
| Comprar itens | 1. Cliente insere seu cartão no caixa eletrônico. <br>2. Sistema exibe menu de operações disponíveis. <br>3. Cliente indica que deseja realizar um saque. <br>4. Sistema apresenta solicitação de senha. <br>5. Cliente digita senha. <br>6. Sistema solicita quantia a ser sacada. <br>7. Cliente retira a quantia e recibo. |

Descrições do tipo **Expandido (ou Completo)** geralmente são escritos em um formato "conversacional" (ou interativo) entre os atores e o sistema. Essas descrições são divididas entre 3 partes:

- Parte 1: Resumo
- Parte 2: Sequência Típica de Eventos
- Parte 3: Sequências Alternativas

Observe um exemplo **Expandido (ou Completo)** Parte 1: Resumo

| Caso de uso | Atores e interesses | Tipo | Referências | Objetivo |
| --- | --- | --- | --- | --- |
| Comprar itens com dinheiro | Cliente (iniciador): deseja obter produtos por meio da compra com dinheiro<br>Caixa: deseja efetuar a venda de produtos de forma segura | Primário | Requisitos R1, R2, R3, R7, R9 | Capturar a venda e seu pagamento em dinheiro |

Observe um exemplo **Expandido (ou Completo)** Parte 2: Sequência Típica

| Ator | Sistema |
| --- | --- |
| 1. Este caso de uso começa quando o Cliente chega ao TPV com itens para comprar |  |
| 2. O Caixa registra o identificador de cada item. Se há mais de um do mesmo item, o caixa também entra a quantidade | 3. Determina o preço do item e adiciona informação sobre o item à transação de venda corrente. A descrição e o preço do item são apresentados |
| 4. Quando termina a entrada dos itens, o Caixa indica ao TPV que as entradas estão completas | 5. Calcula e apresenta o total da venda |
| 6. O Caixa informa o total ao cliente |  |
| 7. O cliente escolhe o tipo de pagamento: <br>1. Se for paamento em dinheiro, ver seção *Pagamento em Dinheiro* <br>2. Se for pagamento por cartão de crédito, ver seção *Pagamento por Cartão de Crédito*<br>3. Se for pagamento por cheque, ver seção *Pagamento em Cheque* |  |
|  | 8. Registra a venda completada |
| 9. O Caixa entrega ao cliente o recibo impreso ao Cliente |  |
| 10. O Cliente sai com os itens comprados |  |

Observe um exemplo **Expandido (ou Completo)** Parte 3: Sequência alternativa

(falta falar sobre pontos de decisão e sequência alternativa)

<Terminar...>



## Diagrama de Sequência do Sistema

Um Diagrama de Sequência do Sistema ilustra os eventos de entrada e saída do sistema. Para uma sequência específica de eventos d eum caso de uso, o diagrama mostra:

- Atores que interagem com o sistema
- O sistema, como uma "caixa-preta", sem detalhes técnicos
- Eventos gerados pelos atores
- Eventos entre sistemas
- Operações de resposta do sistema
- A ordem dos eventos

### "Como fazer" o DSS

> #### Nota Informal
> Basicamente esse ngc tem q descrever as interações do usuario com o sistema e falar como o sistema responde dependendo da interação, ai tipo tu pode clc uma linha vertical representando o usuario e outra representando o sistema, ai tu faz as setas nomeando qual interação ou resposta é representada por aquela linha

#### Traçando interações

Iniciando algo: Linha contínua
Respondendo algo: Linha tracejada

Sempre assumir que o sistema começa na tela inicial

1 diagrama de sequencia pra cada caso de uso

#### Laços e condicionais

É possível que seja representado um laço de repetição ou um ponto de decisão em um siagrama de sequência, para isso deve-se fazer um quadro marcado no canto superior esquerdo com o tipo do quadro, como por exemplo "laço".

No caso do laço especificamente, logo abaixo ao ao lado da descrição "Laço", deve-ser descrever quando esse laço deve finalizar sua repetição.

No caso da tomada de decisão, o quadro deve ser dividido com uma linha horizontal (separando baixo e cima), deve ter a marcação "Alternativa" no canto superior esquerdo do quadro, e semelhante à condição de repetição do quadro de laço, deve ter uma marcação no canto do quadro definindo quais são as condições da tomada de decisão. Cada divisão do quadro deve descrever o que acontece caso cada alternativa seja escolhida.

#### Outros Atores

É possível que o sistema interaja com mais atores que nem são o cliente e nem fazem parte do sistema em si. Para isso, é possível adicionar outros atores com mais linhas verticais representando eles. Todas as outras mecânicas explicadas anteriormente são válidas com esses novos atores.

> Observação: É importante tomar cuidado para não adicionar atores e interações desnecessárias no diagrama, uma vez que a intenção do diagrama é justamente entender como o processo vai funcionar no sistema, então pode ser que algum ator tenha um papel importante no processo, mas que não seja algo que está diretamente relacionado ao funcionamento do sistema, portanto não há necessidade de descrever.

#### Passagem de parâmetros

É possível que uma determinada ação tenha algum parâmetro importante de ser passado. Nesse caso estes parâmetros podem ser passados logo ao lado da descrição das interações, entre parênteses. Essa passagem de parâmetros é válida tanto para o incicio de uma ação quanto para uma resposta, mas geralmente não costuma aparecer em respostas.

> Exemplo: Ao adicionar um produto ao carrinho de uma loja virtual, por exemplo, é válido passar para o sistema qual o ID e a quantidade do produto a ser adicionado

##### Parâmetros opcionais

É possível definir um parâmetro como opcional de forma explícita através de uma conexão de uma caixa marcada como "Opcional" até o parâmetro em questão

#### Reutilização de Diagrama de Sequência

Caso você note durante o desenvolvimento do diagrama que tem uma certa parte que é exatamente igual e se repete várias vezes, é possível demarcar um quadro como "Referência" e dentro dele você descreve qual diagrama acontece naquela posição. E separado, você pode criar esse outro diagrama que vai substituir o quadro de referência em questão.