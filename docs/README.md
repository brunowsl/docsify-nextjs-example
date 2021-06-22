This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Casos de Uso

Referem-se aos serviços, tarefas ou funções que podem ser utilizadas de alguma maneira pelos usuários do sistema;

Representados na forma de elipses com texto interno descrevendo a que serviço o caso de uso se refere.

## Associações

Representam as interações ou relacionamentos entre os casos de uso:  
    **Inclusão.**  
    **Extensão.**  
    **Generalização.**   

– Os atores e os casos de uso Indica que este ator pode usar a função do sistema representada pelo caso de uso;

– Os atores que fazem parte do diagrama:  
    **Generalização**

## Especificação de um Caso de Uso

Casos de uso são requisitos principalmente funcionais, mas podem registrar outros (não funcionais);

Casos de uso são documentos textuais, mas a UML define um diagrama diagrama de casos de uso para ilustrar ilustrar o sistema de uma forma geral:  
– Nomes dos casos de uso;  
– Nomes dos atores e interação dos mesmos com o sistema;  
– Relacionamentos entre casos de uso.

## Tipos e Formatos de Casos de Uso

Casos de uso caixa preta (omitem o comportamento interno) – mais comuns e recomendados.

Exemplo do estilo:  
– Recomendado Recomendado: o sistema sistema registra registra a venda;  
– Não Recomendado: o sistema grava a venda em um banco de dados (ou mesmo, gera uma instrução INSERT).

## Exemplo de caso de uso

### Caso de Uso CDU1: Processar Venda

#### Interessados e Interesses:
Caixa: deseja entrada rápida, precisa e sem erros, de pagamento, pois a falta de dinheiro na gaveta do caixa será deduzida do seu salário.

#### Pré-condições:
O caixa é identificado e autenticado.

#### Garantias de Sucesso (pós-condições):   
A Venda é salva. Os impostos são corretamente calculados. A contabilidade e o Estoque são atualizados. As Comissões são registradas. O recibo é gerado. As aprovações de pagamento são registradas.

#### Cenário de Sucesso Principal (ou Fluxo Básico):

1. O Cliente chega ao PDV com os bens e/ou serviços que deseja adquirir.
2. O Caixa inicia uma nova Venda.
3. O Caixa digita o identificador do item.
4. O sistema registra a linha de item da venda e apresenta uma descrição do item, o seu preço e o total parcial para a venda. O preço é calculado segundo um conjunto de regras de preços.
5. O Caixa repete os passos 3 e 4 até que indique ter terminado.

#### Extensões (ou Fluxos Alternativos):   
##### A qualquer momento o sistema falha:   
Para suportar a recuperação e a correta contabilização, garanta que todas as informações de estado sensíveis das transações transações e todos os eventos eventos possam ser recuperados a partir de qualquer passo do cenário.

#### Requisitos Especiais:   
Interface com o Usuário por tela sensível ao toque em um monitor de painel grande. O texto deve ser visível a uma distância de 1 metro.

#### Lista de Variações Variações Tecnológicas Tecnológicas e de Dados:   
Identificador de item inserido por leitora de código de barras, se estistir.

##### Freqüência de Ocorrência:  
Poderia ser quase contínuo.  
##### Problemas em Aberto:  
Quais as variações nas leis de impostos?

## Como Encontrar Atores, Objetivos e Casos de Uso?

### Casos de uso são identificados para satisfazer aos objetivos de usuário dos atores principais:
Escolher a fronteira do sistema;  
Identificar os atores principais;  
aqueles que devem ter objetivos de usuário;  
Para cada um, identifique os objetivos de usuário;  
Defina casos de uso de satisfaçam os objetivos dos usuários, nomeie-os de acordo com o objetivo.

Inicialmente redija os casos de uso no estilo essencial – sem levar em consideração aspectos da interface com o usuário;

O estilo concreto – deixa claro no texto decisões sobre a interface com o usuário – próprio para as fases seguintes à concepção/iniciação.

## Diagrama de Casos de Uso

O que é?  
– Diagrama pertencente a UML.

Objetivos  
– Apresentar uma visão externa geral das funções e serviços que o sistema vai oferecer aos usuários;
– Atuar como ferramenta na etapa de levantamento de requisitos.

## Atores

- Um diagrama de casos de uso é composto basicamente por atores e casos de uso;
- Os atores representam os papéis desempenhados pelos diversos usuários que poderão utilizar o sistema;
- Um ator pode representar um hardware especial ou mesmo outro sistema;
- Em suma: qualquer agente externo que interaja com o sistema.

## Relacionamento de Generalização/Especialização

• Relaciona casos de uso com características semelhantes e pequenas diferenças entre si;
• Nesses casos é definido um caso de uso geral e definir casos de uso que são especializações deste;
• Neste caso evita-se a redação das partes genéricas em mais de um caso de uso, a redação dos casos de uso especializados se concentra nas diferenças.


## Aprenda Mais

Para aprender mais sobre Casos de Uso para desenvolvimento de softwares acesse este [Link](https://www.dca.ufrn.br/~anderson/FTP/dca0120/P2_Aula3.pdf)
