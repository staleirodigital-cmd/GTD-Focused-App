# Captura — revisão de experiência e jornada

Objetivo: tirar algo da cabeça com mínima decisão, ter confiança de que foi guardado e retomar o contexto anterior. Revisão especializada apoiada em cenários reproduzidos no navegador (390×844 touch, janela 390×520 e desktop); não é pesquisa com participantes nem teste de teclado/Safari físico. Aplicativo não alterado.

Acertos confirmados: abertura com foco no texto; global inicia na Inbox inclusive a partir de outro contexto; Adicionar item parte da lista atual; destino opcional; criação inline mantém texto; guardar em outro destino mantém a página anterior e devolve foco ao botão de captura. Fluxo inicial não exige projeto, contexto, datas ou IA.

Prioridades:
- P0 confiança: falha de localStorage mostra “Guardado em Inbox”, fecha janela e exibe registro apenas em memória. Corrigir sucesso condicional à persistência e preservar texto no erro.
- P1 recuperação: ×/Escape da captura descartam texto; reabrir volta vazio. Preferir recuperação silenciosa do rascunho a confirmação a cada fechamento.
- P1 intenção: Enter grava imediatamente no textarea, inclusive modo mobile. Pode enviar antes de terminar anotação multilinha; revisão de interação deve considerar botão explícito, retorno para nova linha e atalho desktop anunciado, além de composição de texto.
- P2 acesso: menu mobile cobre botão global; capturar enquanto explora listas exige sair da navegação. Avaliar acesso leve sem duplicar elementos visualmente iguais ao Nova lista.
- P2 encontrar destino: busca por “proximas” não encontra “Próximas ações”, diferente do seletor de localização já corrigido. Normalizar acentos.
- P2 captura em sequência: guardar fecha a janela, exigindo reabertura por ideia. Oportunidade para alternativa discreta de continuar capturando; não pressupor que toda captura deve permanecer aberta.

Validação pendente no aparelho: abertura efetiva do teclado pelo foco programático, ditado, botão Retorno, viewport com teclado e gestos de fechar. Janela reduzida manteve botão Guardar visível, mas não prova comportamento do teclado nativo.

Direção: manter tela simples, destino progressivo e ausência de classificação obrigatória. Resolver primeiro confiança e recuperação. Voz/IA e recursos adicionais não são pré-requisitos dessa jornada.

## Implementação após alinhamento
Usuário manteve Enter para guardar no título e pediu nota, data, tags e checklist progressivos inspirados no Things. Implementadas gravação com confirmação real, recuperação silenciosa, histórico de escrita no compositor, acesso global no menu, busca tolerante e captura contínua opcional. Enter em nota continua nova linha e Tab navega. Testes em tests/capture-upgrade.cjs cobrem persistência, falhas, teclado, rascunho, tags e criação de lista; verificação do teclado iOS continua com usuário no aparelho.
