========================================================================
SISTEMA DE GERENCIAMENTO DE ALUGUEL DE JOGOS (DASHBOARD)
========================================================================

Este projeto consiste em uma aplicação interativa para gerenciar o status 
de aluguel de jogos de tabuleiro através de um painel web (Dashboard). O 
script dinamicamente atualiza o estado visual do jogo (se está disponível 
ou alugado), controla os textos dos botões e mantém uma contagem em tempo 
real do total de jogos atualmente alugados, incluindo uma verificação de 
confirmação de segurança antes da devolução de qualquer item.

------------------------------------------------------------------------
1. FUNCIONALIDADES PRINCIPAIS
------------------------------------------------------------------------
* Alternância de Status: Permite alugar ou devolver um jogo com um único 
  clique, modificando as classes CSS correspondentes para a estilização.
* Confirmação de Segurança: Exibe um alerta de confirmação (confirm) antes 
  de processar a devolução de um jogo, evitando ações acidentais.
* Contador Dinâmico: Mantém o controle preciso da quantidade de jogos 
  locados e exibe essa informação no console do navegador.
* Inicialização Automática: Ao carregar a página (DOMContentLoaded), o 
  sistema mapeia o DOM e contabiliza os jogos que já iniciaram com o 
  status de alugados.

------------------------------------------------------------------------
2. ESTRUTURA DO CÓDIGO JAVASCRIPT
------------------------------------------------------------------------
* `jogosAlugados` (Variável Global): Armazena o número inteiro de jogos 
  atualmente marcados como alugados.
* `contarEExibirJogosAlugados()`: Função responsável por imprimir no 
  console a métrica atualizada de locações.
* `alterarStatus(id)`: Função central que recebe o identificador do jogo, 
  manipula as classes de estilização da imagem e do botão, altera o 
  texto de exibição e incrementa/decrementa o contador global.
* `DOMContentLoaded` (EventListener): Garante a sincronização inicial 
  entre o estado pré-renderizado no HTML e a lógica do JavaScript.

------------------------------------------------------------------------
3. TECNOLOGIAS UTILIZADAS
------------------------------------------------------------------------
* 🟡 JavaScript (ES6+) - Lógica de programação e manipulação do DOM.
* 🌐 HTML5 - Estruturação e semântica dos elementos do Dashboard.
* 🎨 CSS3 - Classes de estilização para alternância de estados visuais.

------------------------------------------------------------------------
4. REFERÊNCIA DO PROJETO
------------------------------------------------------------------------
Este projeto foi desenvolvido com base no seguinte treinamento:
* Instituição: Alura
* Curso: Lógica de programação: Praticando com desafios

========================================================================
Criado para fins educacionais e consolidação de manipulação de DOM.
========================================================================
