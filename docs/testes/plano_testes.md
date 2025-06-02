# Plano de Testes

## Histórico de Revisões

| Data       | Versão | Descrição                | Autor  |
| ---------- | ------ | ------------------------ | ------ |
| 02/06/2025 | 1.0    | Versão inicial           | Grupo  |
| DD/MM/AAAA | 1.1    | [Descrição da alteração] | Grupo  |

## 1. Introdução

### 1.1 Objetivos

Garantir que o jogo da velha web funcione corretamente em diferentes cenários, validando a funcionalidade básica do jogo, detecção de vitória, empate, validação de jogadas e reinício da partida.

### 1.2 Escopo

Testar a aplicação web do jogo da velha com as funcionalidades de iniciar jogo, fazer jogadas válidas, detectar vitória e empate, impedir jogadas inválidas, reiniciar partida e suporte para jogar contra outro jogador ou contra a máquina.

### 1.3 Definições, Acrônimos e Abreviações

- UI: Interface do Usuário
- CT: Caso de Teste

## 2. Estratégia de Teste

### 2.1 Níveis de Teste

#### 2.1.1 Testes Unitários

Testar funções JavaScript isoladas, como validação de jogadas, verificação de vitória e empate.

#### 2.1.2 Testes de Integração

Verificar a interação entre os componentes do front-end (HTML, CSS, JS) e o fluxo geral do jogo.

#### 2.1.3 Testes de Sistema

Executar partidas completas simulando o uso real do jogo para validar todos os requisitos funcionais.

#### 2.1.4 Testes de Aceitação

Validar o jogo com usuários finais para garantir que atende às expectativas e funciona corretamente.

### 2.2 Tipos de Teste

#### 2.2.1 Testes Funcionais

Verificar se todas as funcionalidades básicas do jogo estão operando conforme esperado.

#### 2.2.2 Testes de Performance

Avaliar o tempo de resposta da interface e a fluidez das animações durante o jogo.

#### 2.2.3 Testes de Segurança

Verificar se o código JavaScript não permite ações que possam quebrar o jogo ou causar comportamento inesperado.

#### 2.2.4 Testes de Usabilidade

Avaliar a facilidade de uso da interface e clareza das mensagens para o usuário.

#### 2.2.5 Testes de Regressão

Reexecutar casos de teste após atualizações para garantir que funcionalidades antigas continuem funcionando.

## 3. Recursos

### 3.1 Ambientes de Teste

- Navegadores: Chrome, Firefox, Edge, Safari (versões atuais)
- Dispositivos: Desktop e mobile (responsividade)

### 3.2 Ferramentas

- Navegadores com ferramentas de desenvolvedor
- Mermaid Live Editor (para diagramas, se necessário)
- Ferramentas de captura de tela e gravação para documentação

### 3.3 Equipe

| Código  | Tarefa                        | Responsáveis                                                                             |
| ------- | ----------------------------- | ---------------------------------------------------------------------------------------- |
| SCRUM-1 | Pesquisa Qualitativa          | Márcio Henrique, João Pedro Tadei, Maria Fernanda (Auxiliadora), Isadora Rocha (Revisão) |
| SCRUM-2 | Definição do "Sistema Seguro" | Manuella Cotrín, Laíse Garcia, Maria Fernanda (Auxiliadora), Isadora Rocha (Revisão)     |
| SCRUM-3 | Design                        | João Antônio Marini, Maria Fernanda (Auxiliadora), Isadora Rocha (Revisão)               |


## 4. Cronograma

| Atividade                  | Início     | Término    |
| -------------------------- | ---------- | ---------- |
| Planejamento do Teste      | 10/02/2025 | 20/02/2025 |
| Desenvolvimento dos testes | 21/02/2025 | 30/04/2025 |
| Execução dos testes        | 01/05/2025 | 31/05/2025 |
| Análise e relatório        | 01/06/2025 | 02/06/2025 |

## 5. Critérios

### 5.1 Critérios de Entrada

1.Código fonte estável e funcional para execução do jogo
2.Ambiente de teste configurado e disponível

### 5.2 Critérios de Saída

1.Todos os casos de teste críticos foram executados com sucesso ou registrados os incidentes
2.Bugs críticos corrigidos e retestados

### 5.3 Critérios de Suspensão e Retomada

1.Suspensão: quando bugs críticos bloqueiam a continuidade dos testes
2.Retomada: após correção dos bugs e validação da estabilidade

## 6. Matriz de Risco e Contingência

| Risco                             | Probabilidade | Impacto | Estratégia de Mitigação               |
| --------------------------------- | ------------- | ------- | ------------------------------------- |
| Bugs críticos no fluxo de jogo    | Média         | Alto    | Priorizar correção imediata           |
| Incompatibilidade com navegadores | Baixa         | Médio   | Testar em múltiplos browsers          |
| Falha no ambiente de teste        | Baixa         | Alto    | Ter ambientes alternativos preparados |

## 7. Casos de Teste

| ID   | Descrição                          | Requisito | Pré-condições                      | Passos                            | Resultado Esperado                                    | Prioridade |
| ---- | ---------------------------------- | --------- | ---------------------------------- | --------------------------------- | ----------------------------------------------------- | ------|
| CT01 | Jogar partida completa com vitória | REQ-001   | Jogo iniciado, tabuleiro vazio     | Fazer jogadas válidas até vitória | Vitória detectada e mensagem exibida corretamente     | Alta  |
| CT02 | Jogar partida completa com empate  | REQ-001   | Jogo iniciado, tabuleiro vazio     | Fazer jogadas válidas até empate  | Empate detectado e mensagem exibida corretamente      | Alta  |
| CT03 | Tentar jogar em célula ocupada     | REQ-002   | Partida em andamento               | Tentar marcar célula já ocupada   | Jogada inválida rejeitada e mensagem de aviso exibida | Alta  |
| CT04 | Reiniciar partida                  | REQ-004   | Partida finalizada ou em andamento | Clicar em "Reiniciar Jogo"        | Tabuleiro limpo e jogo reiniciado                     | Média |


## 8. Métricas

1.Percentual de casos de teste executados com sucesso
2.Tempo médio para execução dos testes
3.Número de defeitos encontrados por tipo e gravidade

## 9. Relatórios

1.Percentual de casos de teste executados com sucesso
2.Tempo médio para execução dos testes
3.Número de defeitos encontrados por tipo e gravidade

## 10. Aprovação

| Nome                | Papel                           | Assinatura | Data       |
| ------------------- | ------------------------------- | ---------- | ---------- |
| Maria Fernanda      | Analista QA / Auxiliadora       |            | 02/06/2025 |
| Isadora Rocha       | Revisora                        |            | 02/06/2025 |
| Márcio Henrique     | Pesquisador                     |            | 02/06/2025 |
| João Pedro Tadei    | Pesquisador                     |            | 02/06/2025 |
| Manuella Cotrim     | Desenvolvedora / Sistema Seguro |            | 02/06/2025 |
| Laíse Garcia        | Desenvolvedora / Sistema Seguro |            | 02/06/2025 |
| João Antônio Marini | Designer                        |            | 02/06/2025 |

>[!WARNING]
>A execução completa do plano de testes é essencial para garantir a qualidade do software. Qualquer desvio do plano deve ser documentado e justificado.
