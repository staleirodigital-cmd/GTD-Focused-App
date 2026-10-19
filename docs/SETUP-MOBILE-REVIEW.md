# Revisão de setup mobile

Revisão especializada de experiência/jornada, apoiada por verificações técnicas e de interface em Chromium com toque emulado, 390×844 e janela reduzida de 360×560. Não equivale a teste em iPhone físico, teclado virtual, Safari/VoiceOver ou pesquisa com participantes. Sem alteração do aplicativo.

Confirmado: primeiro acesso abre Inbox vazia, sem tour ou conteúdo fictício; Nova lista disponível no menu; nome e posição editáveis; criação contextual preenche pai; criar sublista funciona; renomeação preservada ao voltar da localização. Regressões existentes cobrem criação inline durante captura com rascunho preservado, remoção de listas com conteúdo e recarga sem restaurar template apagado.

Achados:
1. Prioridade alta: Nova lista > digitar nome > Dentro de > × fecha a criação e perde o rascunho. Voltar preserva. Há diferença entre voltar de um seletor e abandonar explicitamente a criação, que o fechamento atual não comunica.
2. Prioridade média: localização da lista não oferece busca, ao contrário do destino de item. Com 20+ listas, rolagem e nomes semelhantes dificultam encontrar pai.
3. Prioridade média: após reordenar pelo organizador, o contêiner é reconstruído e o foco volta ao nome, deslocando a rolagem (650 para 591 no caso observado). A pessoa perde a continuidade do botão de ordem.
4. Prioridade média: Lista aqui tem texto de 11px e alvo de 40px, abaixo dos 44px adotados em outros controles de toque.
5. Prioridade baixa: hover da seta de ordenação ainda usa azul antigo. A auditoria visual anterior não cobriu esse estado.
6. Primeiro acesso: a entrada em Inbox vazia é intencionalmente simples; personalizar exige descobrir o menu. Avaliar com o usuário a descobribilidade antes de adicionar qualquer convite/tour.

Não propor novo onboarding obrigatório, categorias fixas, campos adicionais ou classificação de projetos. Pendentes no dispositivo real: teclado cobrindo botões, zoom dos campos, áreas seguras e Safari.

## Correções executadas
Os cinco achados foram ajustados por autorização do usuário. Regressão em tests/setup-mobile-fixes.cjs cobre retorno com rascunho por ×/Escape/Voltar, busca sem acentos e estado vazio, alvo contextual de 44px, rolagem/foco na reordenação e cores das setas nos dois temas. A avaliação de experiência continua incluindo descobribilidade e oportunidades; testes automatizados não substituem a revisão no aparelho ou com participantes.
