> **Atividade acadêmica** realizada durante o curso de Game QA Testing (CultSP Pro), em grupo, com fins de aprendizado — não é um teste profissional/comercial contratado. Nomes de jogadores identificados apenas como "Participante N" nesta versão pública.

# Playtest UX Report — Brasas

**Jogo:** Brasas (RPG tático)
**Meu papel:** Pesquisa e Análise — condução da síntese dos achados a partir das sessões de teste
**Metodologia:** Teste exploratório moderado e remoto (pré-entrevista → gameplay observado → pós-entrevista)
**Sessão:** 1 sessão em grupo, ~45 minutos, 4 participantes, Windows
**Nota média dos participantes:** 5,0 / 10

## Perfil dos participantes

| Participante | Perfil | Nota |
|---|---|---|
| Participante 1 | Casual | 5/10 |
| Participante 2 | Casual | 5/10 |
| Participante 3 | Casual/Competitivo | 6/10 |
| Participante 4 | Casual | 4/10 |

## Escala de severidade utilizada

| Nível | Critério |
|---|---|
| **Crítica** | Impede ou desestimula fortemente a continuidade do jogador. Ação urgente. |
| **Séria** | Atrapalha/irrita significativamente parte dos jogadores. Corrigir assim que possível. |
| **Média** | Frustra/incomoda, mas não impede a conclusão da tarefa. |
| **Baixa** | Ajuste estético/pontual. Isoladamente trivial, mas acumulado afeta a credibilidade. |
| **Positiva** | Funcionou como esperado e foi bem recebido. Deve ser preservado. |

## Achados

| ID | Título | Severidade | Status |
|---|---|---|---|
| PT-001 | Performance e tempo de carregamento | Crítica | Reportado |
| PT-002 | Caminho travado na locomoção | Crítica | Reportado |
| PT-003 | Legibilidade e ritmo dos textos (FTUE) | Séria | Reportado |
| PT-004 | Encerramento de turno não é intuitivo | Séria | Reportado |
| PT-005 | Classe Arqueiro — expectativa visual x mecânica real | Séria | Reportado |
| PT-006 | Sistema de pontos de movimento sem indicador visível | Séria | Reportado |
| PT-007 | Direção de arte, personagens e ambientação | Positiva | Confirmado |

---

### PT-001 — Performance e tempo de carregamento
**Severidade:** Crítica

**Ocorrência:** Dois jogadores relataram demora no carregamento do jogo. Para um deles, a demora foi grande o suficiente para exigir o fechamento e a reabertura do jogo.

**Impacto no jogo:** Precisar reabrir o jogo interrompe a sessão de forma abrupta — é o tipo de fricção que mais desestimula um jogador a continuar testando ou jogando.

---

### PT-002 — Caminho travado na locomoção
**Severidade:** Crítica

**Ocorrência:** Foi identificado um caminho onde o personagem trava e não consegue se locomover, impedindo a continuidade normal da movimentação.

**Impacto no jogo:** Um bloqueio de movimentação interrompe diretamente o progresso do jogador dentro da partida, podendo forçar o abandono da sessão.

---

### PT-003 — Legibilidade e ritmo dos textos (FTUE)
**Severidade:** Séria

**Ocorrência:** As legendas da introdução avançam rápido demais para leitura completa. O cabeçalho do tutorial em texto também ultrapassa o espaço disponível na interface, e o tamanho da fonte não atraiu os jogadores — inclusive os que não costumam ler notaram que, neste caso, a leitura seria importante.

**Impacto no jogo:** A perda de informação no início do jogo (FTUE) compromete o entendimento das mecânicas, obrigando os jogadores a aprender por tentativa e erro em vez de pela orientação pretendida.

---

### PT-004 — Encerramento de turno não é intuitivo
**Severidade:** Séria

**Ocorrência:** Não ficou claro para os jogadores que era necessário pressionar manualmente "Encerrar turno". Um dos jogadores descreveu a experiência como confusa e só descobriu a mecânica após clicar em tudo disponível na tela.

**Impacto no jogo:** A falta de clareza atrasa o aprendizado do fluxo central de combate.

**Recomendação:** Os próprios jogadores sugeriram encerramento automático quando todas as ações do turno forem consumidas.

---

### PT-005 — Classe Arqueiro: expectativa visual x mecânica real
**Severidade:** Séria

**Ocorrência:** Os jogadores identificaram que o arqueiro precisa se aproximar dos inimigos para atacar, com alcance muito próximo ao de uma classe corpo a corpo (espada).

**Impacto no jogo:** A identidade visual do arqueiro cria uma expectativa natural de combate à distância. Se essa não for a proposta da classe, o jogo precisa comunicar melhor qual é o seu diferencial estratégico.

*Observação analítica: este achado é um bom exemplo de como um problema de UX pode nascer do próprio game design (a leitura visual da classe), e não apenas de bug ou interface.*

---

### PT-006 — Sistema de pontos de movimento sem indicador visível
**Severidade:** Séria

**Ocorrência:** Não existe um sistema visível que indique quantos pontos de movimento o personagem ainda possui durante o turno.

**Impacto no jogo:** Sem essa referência, os jogadores têm dificuldade em planejar deslocamentos com segurança, o que enfraquece a camada estratégica pretendida para um RPG de turnos.

---

### PT-007 — Direção de arte, personagens e ambientação
**Severidade:** Positiva

**Ocorrência:** A interface e a arte foram destacadas positivamente por múltiplos participantes. Os modelos 3D dos personagens e a ambientação da cidade foram bem recebidos, incluindo a troca de música conforme o bioma.

**Impacto no jogo:** A direção de arte e a ambientação estão gerando conexão emocional genuína com os jogadores — um pilar a ser preservado e reforçado nas próximas iterações, independentemente dos ajustes de UX pendentes.

---

## Conclusão

A direção de arte, os personagens 3D e a ambientação de Brasas foram bem recebidos e geraram conexão real com os jogadores — um ponto forte a preservar. Por outro lado, os testes foram realizados com um FTUE sem onboarding adequado (tutorial em texto rápido demais, sem orientação suficiente na segunda parte), o que explica boa parte da confusão relatada nas mecânicas de turno, movimentação e câmera.

A classe Arqueiro merece atenção especial: o problema não parece ser apenas preferência individual, mas sim uma expectativa criada pela própria identidade visual da classe, que hoje não corresponde ao seu funcionamento real. Os itens críticos (carregamento e caminho travado) devem ser tratados com prioridade, pois interrompem a sessão do jogador. Os demais pontos de severidade Séria reforçam a necessidade de revisar a comunicação das mecânicas antes de investir em novo conteúdo.
