# Caso de Teste: [ID]

## Título

Jogar uma partida do jogo da velha até vitória, empate ou reinício.

## Objetivo

Verificar se o usuário consegue jogar uma partida completa, fazendo jogadas válidas, e se o sistema identifica corretamente vitória, empate e permite reiniciar.

## Requisitos/Histórias Relacionados

- REQ-001: O sistema deve permitir iniciar uma nova partida.
- REQ-002: O sistema deve validar jogadas e impedir jogadas em células ocupadas.
- REQ-003: O sistema deve detectar vitória, empate e exibir mensagem apropriada.
- REQ-004: O sistema deve permitir jogar contra outro jogador ou contra a máquina.

## Pré-condições

1.O usuário acessou a página do jogo da velha.
2.O jogo está carregado e o tabuleiro está vazio.

## Dados de Teste

- Tabuleiro inicial vazio.
- Sequência de jogadas válidas para jogador 1 e jogador 2 (ou máquina).
- Jogada inválida tentando marcar célula ocupada.

## Passos

1.Abrir a página do jogo da velha.
2.Escolher o modo de jogo (contra outro jogador ou IA).
3.Jogador 1 realiza a primeira jogada clicando em uma célula vazia.
4.Jogador 2 (ou máquina) realiza a próxima jogada.
5.Continuar alternando jogadas até um jogador vencer ou ocorrer empate.
6.Verificar se o sistema exibe a mensagem correta de vitória ou empate.
7.Tentar realizar jogada em célula já ocupada e verificar se o sistema bloqueia.
8.Clicar em "Reiniciar Jogo" para iniciar uma nova partida.
9.Verificar se o tabuleiro é limpo e pronto para nova partida.

## Resultado Esperado

Jogadas válidas são aceitas e marcadas corretamente no tabuleiro, jogadas em células ocupadas são rejeitadas com aviso, o sistema detecta corretamente vitória e empate, exibindo mensagens apropriadase o botão reiniciar limpa o tabuleiro e reinicia a partida.

## Pós-condições

1.O jogo termina com resultado (vitória ou empate) exibido.
2.O usuário pode iniciar uma nova partida a qualquer momento.
3.O tabuleiro está em estado consistente para nova partida.

## Tipo de Teste

Sistema / Funcional

## Automação

Manual (pode ser automatizado futuramente com testes UI)

## Prioridade

Alta

## Observações

Testar em diferentes navegadores para verificar compatibilidadee validar mensagens exibidas para acessibilidade.
