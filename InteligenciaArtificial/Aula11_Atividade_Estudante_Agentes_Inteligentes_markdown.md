# Atividade sobre agentes inteligentes

Aula 19/10/2026 | Professora Kadidja Valéria | Inteligência artificial

**Disciplina:** Inteligência Artificial, Linguagens Formais e Autômatos

**Estudante:** [nome] | **Turma:** [turma]

Realize os exercícios 2.3, 2.4 e 2.5 do Capítulo 2 sobre agentes inteligentes. Analise a racionalidade, descreva ambientes de tarefa por meio do modelo PEAS e explique os conceitos com suas próprias palavras. Utilize o capítulo disponibilizado e justifique suas respostas.

**Modalidade sugerida:** individual com consulta. **Tempo estimado:** 2h30. **Prazo:** conforme orientação da professora.

## Preparação
Leia os tópicos sobre racionalidade, ambientes e estrutura dos agentes, especialmente a Seção 2.3.2.

## Exercício 2.3
Para cada afirmação, indique V ou F, justifique e forneça exemplo ou contraexemplo. Explicite as hipóteses utilizadas.

### a. Um agente que detecta apenas informações parciais sobre o estado não pode ser perfeitamente racional.
- Falso
- Um agente pode ser racional mesmo com informações parciais.
- robô aspirador que limpa a sujeira detectada.

### b. Existem ambientes de tarefa nos quais nenhum agente reativo puro pode comportar-se racionalmente.

- Verdadeiro
- Um agente reativo puro pode falhar quando precisa lembrar o passado.
- robô perdido em um labirinto.

### c. Existe um ambiente de tarefa em que todo agente é racional.

- Verdadeiro.
- Se todas as ações forem igualmente boas, qualquer agente será racional.
- botões que geram o mesmo resultado.

### d. A entrada para o programa de agente é a mesma que a entrada para a função de agente.

- Falso
- A função recebe o histórico de percepções; o programa recebe a percepção atual.
- histórico completo versus visão atual.

### e. Toda função de agente é implementável por uma combinação de programa/máquina.

- Falso
- Nem toda função pode ser implementada por um programa.
- função que exige cálculos impossíveis de executar em tempo finito.

### f. Suponha que um agente selecione sua ação uniformemente ao acaso do conjunto de ações possíveis. Existe um ambiente de tarefa determinista em que esse agente é racional.

- Verdadeiro.
- Se todas as ações forem igualmente boas, escolher ao acaso é racional.
- todas geram a mesma recompensa.

### g. É possível para um dado agente ser perfeitamente racional em dois ambientes de tarefa distintos.

- Verdadeiro
- Um agente pode ser racional em ambientes diferentes.
- ficar parado quando essa é a melhor ação nos dois ambientes.

### h. Todo agente é racional em um ambiente não observável.

- Falso.
- Não observar o ambiente não garante racionalidade.
- robô que avança no escuro e bate em obstáculos.

### i. Um agente jogador de pôquer perfeitamente racional nunca perde.

- Falso.
- Um jogador racional pode perder por causa da sorte.
- o adversário recebe cartas melhores.

## Exercício 2.4
Para cada caso, delimite o agente, preencha o PEAS e justifique todas as classificações. Considere Titã como cenário hipotético do exercício.

### Caso 1 — Jogar futebol.

- Agente analisado: Jogador de futebol individual.
- Objetivo e hipóteses: Ajudar a equipe a vencer uma partida, respeitando as regras.
- P — Medida de desempenho: Gols, assistências, passes certos e contribuição para a vitória.
- E — Ambiente: Campo, bola, companheiros, adversários, árbitro e gol.
- A — Atuadores: Pernas, pés, cabeça e movimentos do corpo.
- S — Sensores: Visão, audição e percepção da posição da bola e dos jogadores.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade |Parcialmente observável | o jogador não vê tudo o que ocorre no campo. |
| Número de agentes | Multiagente | cooperativo com companheiros e competitivo com adversários. |
| Previsibilidade | Estocástico | as ações dos outros jogadores tornam os resultados incertos. |
| Dependência entre decisões | Sequencial | cada ação influencia as seguintes. |
| Mudança durante a decisão | Dinâmico | o jogo continua enquanto o jogador decide. |
| Natureza dos elementos | Contínuos e discretos | movimentos contínuos e regras ou eventos discretos. |
| Conhecimento do funcionamento | Conhecido | regras são conhecidas, embora os resultados sejam incertos. |

### Caso 2 — Explorar os oceanos subterrâneos de Titã.

- Agente analisado: Robô autônomo de exploração submarina.
- Objetivo e hipóteses: Mapear o oceano hipotético, coletar amostras e identificar possíveis sinais de vida.
- P — Medida de desempenho: Área mapeada, amostras coletadas, descobertas e segurança do robô.
- E — Ambiente: Oceano subterrâneo, água, rochas, obstáculos e organismos hipotéticos.
- A — Atuadores: Propulsores, braços robóticos e instrumentos de coleta.
- S — Sensores: Câmeras, sonar, sensores de pressão, temperatura e composição química.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade |Parcialmente observável | os sensores não revelam tudo o que existe no oceano. |
| Número de agentes | Agente único | considera-se apenas um robô autônomo. |
| Previsibilidade | Estocástico | correntes e condições ambientais podem variar. |
| Dependência entre decisões | Sequencial| cada movimento influencia a exploração seguinte. |
| Mudança durante a decisão | Dinâmico | as condições podem mudar durante a operação. |
| Natureza dos elementos | Contínuos e discretos | movimento contínuo e objetivos discretos de exploração. |
| Conhecimento do funcionamento | Desconhecido | o robô não conhece completamente as condições desse oceano hipotético. |

### Caso 3 — Comprar livros usados de IA na Internet.

- Agente analisado: Programa de compras automatizadas.
- Objetivo e hipóteses: Comprar livros relevantes, em bom estado e pelo menor preço possível.
- P — Medida de desempenho: Preço total, qualidade, relevância e entrega bem-sucedida
- E — Ambiente: Sites de vendas, livros, vendedores, anúncios e sistema de pagamento.
- A — Atuadores: Cliques, pesquisas, filtros e comandos digitais de compra e pagamento.
- S — Sensores: Resultados de busca, preços, descrições, fotos, avaliações e informações de entrega.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade | Parcial | o estado real do livro pode diferir do anúncio. |
| Número de agentes | Multiagente | há vendedores e outros compradores. |
| Previsibilidade | Estocástico | a disponibilidade e os preços podem mudar. |
| Dependência entre decisões | Sequencial | pesquisar, comparar e comprar são etapas relacionadas. |
| Mudança durante a decisão | Dinâmico |os produtos podem ser vendidos durante a pesquisa. |
| Natureza dos elementos | Discretos e contínuos | anúncios são discretos e preços são numéricos.|
| Conhecimento do funcionamento | Conhecido | as regras do site podem ser conhecidas, embora as condições reais dos livros sejam incertas. |

### Caso 4 — Jogar uma partida de tênis.

- Agente analisado: Jogador individual.
- Objetivo e hipóteses: Vencer a partida seguindo as regras.
- P — Medida de desempenho: Pontos, games, sets e vitória
- E — Ambiente: Quadra, bola, rede, adversário e árbitro.
- A — Atuadores: Braços, pernas e raquete.
- S — Sensores: Visão, audição e percepção da bola e do adversário.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade | Parcial | o jogador não conhece todas as intenções do adversário. |
| Número de agentes | Multiagente | os jogadores disputam a vitória. |
| Previsibilidade | Estocástico | as ações do adversário geram incerteza. |
| Dependência entre decisões | Sequencial | cada golpe influencia o seguinte. |
| Mudança durante a decisão | Dinâmico | a bola continua em movimento. |
| Natureza dos elementos | Contínuos e discretos | movimentos contínuos e pontuação discreta. |
| Conhecimento do funcionamento | Conhecido | as regras são conhecidas, mas o resultado é incerto. |

### Caso 5 — Praticar tênis contra uma parede.

- Agente analisado: Jogador individual.
- Objetivo e hipóteses: Melhorar a precisão e a coordenação dos golpes.
- P — Medida de desempenho: Precisão, controle e quantidade de rebatidas consecutivas.
- E — Ambiente: Jogador, bola, raquete, parede e quadra.
- A — Atuadores: Braços, pernas e raquete.
- S — Sensores: Visão, audição e percepção da trajetória da bola.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade | Completa | supondo que a bola e a parede estejam sempre visíveis. |
| Número de agentes | Agente único | a parede não é um agente decisor. |
| Previsibilidade | Determinístico | supondo condições estáveis e conhecidas. |
| Dependência entre decisões | Sequencial | cada golpe depende da trajetória anterior. |
| Mudança durante a decisão | Dinâmico | a bola está em movimento. |
| Natureza dos elementos | Contínuos | posição, velocidade e movimentos variam continuamente. |
| Conhecimento do funcionamento | Conhecido | o jogador conhece a tarefa e os rebotes esperados. |

### Caso 6 — Realizar um salto de altura.

- Agente analisado: Atleta individual.
- Objetivo e hipóteses: Saltar a maior altura possível sem derrubar o sarrafo
- P — Medida de desempenho: Altura alcançada e tentativas válidas.
- E — Ambiente: Pista, colchão, sarrafo e árbitros.
- A — Atuadores: Pernas, braços e movimentos corporais.
- S — Sensores: Visão, equilíbrio e percepção corporal.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade | Parcial | o atleta não percebe perfeitamente todas as variáveis físicas. |
| Número de agentes | Agente único | considera-se apenas a execução individual do salto. |
| Previsibilidade | Estocástico | pequenas variações podem alterar o resultado. |
| Dependência entre decisões | Episódico | cada tentativa pode ser avaliada separadamente. |
| Mudança durante a decisão | Dinâmico | o corpo se movimenta durante o salto. |
| Natureza dos elementos | Contínuos e discretos | altura contínua e tentativas válidas ou inválidas. |
| Conhecimento do funcionamento | Conhecido | as regras são conhecidas, embora o resultado físico seja incerto. |

### Caso 7 — Participar de um leilão de um item, realizando lances.

- Agente analisado: Programa de lances automatizados.
- Objetivo e hipóteses: Comprar o item desejado sem ultrapassar o orçamento.
- P — Medida de desempenho: Adquirir o item pelo menor preço possível, respeitando o orçamento.
- E — Ambiente: Plataforma, item, vendedor e concorrentes.
- A — Atuadores: Envio digital de lances e confirmação de compra.
- S — Sensores: Preço atual, histórico de lances, notificações e tempo restante.

| Propriedade | Classificação | Justificativa |
|---|---|---|
| Observabilidade | Parcial | o agente não conhece todos os limites e as intenções dos concorrentes. |
| Número de agentes | Multiagente competitivo | os participantes disputam o item. |
| Previsibilidade | Estocástico | os outros participantes podem fazer lances inesperados. |
| Dependência entre decisões | Sequencial | cada lance depende dos anteriores. |
| Mudança durante a decisão | Dinâmico | os lances e o tempo restante mudam. |
| Natureza dos elementos | Discretos e contínuos | lances são eventos discretos e o tempo varia continuamente. |
| Conhecimento do funcionamento | Conhecido | supondo que as regras do leilão sejam conhecidas, embora as estratégias dos concorrentes sejam incertas. |

### Opções para classificação
- **Observabilidade:** Completamente observável, parcialmente observável ou não observável.
- **Número de agentes:** Agente único ou multiagente; indique cooperação ou competição quando pertinente.
- **Previsibilidade:** Determinístico ou estocástico; considere a influência estratégica de outros agentes.
- **Dependência entre decisões:** Episódico ou sequencial.
- **Mudança durante a decisão:** Estático, dinâmico ou semidinâmico.
- **Natureza dos elementos:** Discretos, contínuos ou combinação; considere estados, tempo, percepções e ações.
- **Conhecimento do funcionamento:** Conhecido ou desconhecido para o agente.

### Comparação final
1. O que muda entre jogar tênis contra outra pessoa e praticar contra uma parede?
2. Por que comprar livros usados pode exigir decisões com informações incompletas?
3. Como outros agentes influenciam futebol e leilões?

Respostas: 
1.Contra outra pessoa, o ambiente é multiagente e competitivo, pois o adversário toma decisões próprias. Contra a parede, há apenas um agente decisor e os rebotes podem ser previsíveis.

2.Porque fotos, descrições e avaliações podem não mostrar o estado real do livro. Assim, o agente precisa decidir com informações parciais.

3.No futebol, os colegas cooperam e os adversários competem. No leilão, os concorrentes disputam o mesmo item, influenciando os preços e as decisões.

## Exercício 2.5
Defina cada termo com suas palavras em duas a quatro linhas e apresente um exemplo.

### Agente

- Definição: É algo que percebe o ambiente por sensores e age sobre ele por atuadores.
- Exemplo: Um robô aspirador que detecta sujeira e limpa o chão.

### Função de agente

- Definição: É a relação que determina qual ação o agente deve realizar com base nas percepções recebidas.
- Exemplo: Ao detectar sujeira, o agente escolhe aspirar.

### Programa de agente

- Definição: É o software que implementa a função de agente em uma máquina.
- Exemplo: Um programa que recebe informações dos sensores e controla as rodas de um robô.
### Racionalidade

- Definição: É escolher a ação que maximiza o desempenho esperado com base nas informações disponíveis.
- Exemplo: Um robô desvia de um obstáculo para evitar uma colisão.

### Autonomia

- Definição:É a capacidade de agir com base nas próprias percepções e experiências, sem depender apenas de instruções pré-programadas.
- Exemplo: Um aspirador que aprende quais áreas da casa ficam mais sujas.

### Agente reativo

- Definição: Escolhe ações de acordo com a percepção atual, sem precisar considerar um histórico de situações.
- Exemplo: Um robô que recua quando detecta um obstáculo.

### Agente baseado em modelo

- Definição: Mantém uma representação interna do ambiente para estimar estados que não consegue observar diretamente.
- Exemplo: Um robô que memoriza onde existem obstáculos, mesmo quando não consegue vê-los.

### Agente baseado em objetivos

- Definição: [escreva aqui]
- Exemplo: [escreva aqui]

### Agente baseado em utilidade

- Definição: Avalia diferentes resultados conforme o quanto são desejáveis e escolhe a ação com maior utilidade esperada.
- Exemplo: Um programa que escolhe uma rota considerando tempo, distância e segurança.
- 
### Agente com aprendizagem

- Definição:Melhora seu comportamento com base na experiência e nos resultados das ações anteriores.
- Exemplo: Um sistema de recomendações que aprende as preferências do usuário.

## Síntese com autômatos
Escolha um caso do item 2.4. Apresente três estados internos, três percepções, três ações e duas regras no formato estado atual + percepção → próximo estado e ação. Explique como estados internos representam informação passada e cite uma limitação da simplificação.

Resposta: Caso escolhido: Robô aspirador.

Estados internos:

S1: Área desconhecida.

S2: Sujeira detectada.

S3: Área limpa.

Percepções:

P1: Nenhuma sujeira detectada.

P2: Sujeira detectada.

P3: Obstáculo detectado.

Ações:

A1: Avançar.

A2: Aspirar.

A3: Desviar.

Regras de transição:

Estado atual S1 + percepção P2 → próximo estado S2 e ação A2 (aspirar).

Estado atual S2 + percepção P3 → próximo estado S2 e ação A3 (desviar).

Explicação: Os estados internos representam informações guardadas de percepções anteriores, ajudando o robô a decidir mesmo quando não consegue observar todo o ambiente.

Limitação: Esse modelo é simplificado, pois possui poucos estados e não representa todas as situações possíveis de uma casa real.

## Entrega e avaliação
Confira: identificação; nove análises no item 2.3; sete casos completos no item 2.4; dez conceitos no item 2.5; síntese; referências.
Nome sugerido: `NomeSobrenome_Atividade_AgentesInteligentes`. Prazo e envio conforme orientação da professora.

| Critério | Atividade avaliativa (1,0 ponto) A2 |
|---|---:|
| Item 2.3 — correção e argumentação | 30% |
| Item 2.4 — PEAS e classificação justificada | 40% |
| Item 2.5 — precisão conceitual e exemplos | 20% |
| Síntese, organização e referências | 10% |

## Referências
Material-base: Capítulo 2 — Agentes inteligentes, disponibilizado para a aula de 19/10/2026.
Referências adicionais: [registre aqui]
