# Clareza · princípios de produto e experiência

## Premissa central
O usuário avalia a confiança no próprio sistema. A ferramenta guarda, preserva e apresenta fielmente os registros, facilitando captura, esclarecimento, organização, engajamento e revisão. Ausência de ação, texto curto e tempo sem movimento não são diagnósticos de erro. A organização serve à confiança; classificações e métricas não substituem o julgamento da pessoa.

## Liberdade e método
O GTD é praticado pela pessoa. A ferramenta é um espaço aberto para tangibilizar essa prática. A organização inicial é um template editável e removível, incluindo Projetos, Próximas ações, Aguardando, Algum dia/Talvez e seus contextos. Não manter categorias obrigatórias escondidas depois que o usuário as remove.
Listas independentes e listas dentro de listas usam o mesmo modelo. A posição não determina o significado dos itens. Uma lista pode conter itens e outras listas; abrir o conjunto reúne os mesmos registros, sem cópia. Sonhos, referências, checklists ou assuntos podem existir diretamente em Meu espaço.
Projeto é um resultado desejado que exige mais de uma ação, mesmo pequeno e com apenas um próximo passo conhecido. Checklist não determina projeto. A transformação em projeto é explícita; mover para uma lista chamada Projetos não transforma automaticamente um item. A relação entre resultado e ações é independente da organização em listas.

## Experiência e refinamento
Simplicidade extremamente refinada. Mostrar o necessário para o objetivo atual e revelar possibilidades no contexto exato em que ajudam. Tipografia, alinhamento óptico, ritmo, proporção e comportamento consistente têm prioridade sobre decoração. Things é referência de qualidade, não estrutura obrigatória nem identidade a copiar. Iconografia vetorial coerente e própria. O experimento de emojis em todas as listas foi rejeitado pelo usuário. Sem breadcrumb na navegação principal.
Hierarquia por composição de conjuntos: título com mais peso, linhas alinhadas, espaço e divisórias discretas. Não usar encadeamento de recuos em cascata. Profundidades maiores são exploradas dentro das listas; não comprimir tudo na navegação. Destinos têm áreas de toque confortáveis, seleção inequívoca, foco visível e nomes completos acessíveis. Claro/escuro devem tratar fundo, texto, campos e controles como um conjunto.

## Divulgação progressiva
Na lista: título e indicadores úteis. No item: notas e detalhes conforme existam ou sejam solicitados. Opções específicas aparecem ao escolher a operação. Evitar campos vazios, mensagens educativas permanentes, tours, questionários e tarefas fictícias.
Nova lista é um acesso estável e descobrível. Criar lista aqui é contextual e preenche o destino. Não espalhar um + por seção. Em um destino de item, permitir buscar e criar lista sem perder o rascunho. Cancelar a criação deve permitir retomar o encaminhamento.

## Captura e manutenção
O + global e N abrem captura com Inbox como destino inicial, não obrigatório. O usuário pode selecionar qualquer lista ou criar uma na hora. Adicionar aqui parte da lista atual; adicionar uma ação relacionada preserva o vínculo explícito com o projeto. Não converter captura em tarefa/plano/projeto por inferência.
Criar pede nome; localização vem preenchida e é editável sob demanda. Mover para Meu espaço torna a lista independente. Renomear, mover e ordenar são operações comuns, sem burocracia. Arrastar é um atalho no desktop; as opções de localização e os botões de ordem são alternativas explícitas para toque/teclado/acessibilidade. Distinguir visualmente inserir antes, depois e dentro; impedir ciclos; oferecer desfazer.
Remover uma lista nunca apaga silenciosamente seu conteúdo: itens sobem para a lista-pai; sublistas sobem um nível. Se a lista era independente, itens vão para Inbox e sublistas ficam em Meu espaço, com explicação antes da remoção. Lista vazia pode ser removida diretamente com desfazer.
Checklist é uma apresentação opcional da lista. Marcar um item de checklist não significa concluir um compromisso; usar estado de conferência separado. Checklist dentro de um item permanece disponível. Não exigir formato na criação.

## Projetos, datas e revisão
Projetos abrem uma visão do resultado, suporte e lembretes relacionados agrupados pelas listas reais do usuário, sem repetir o nome do projeto em cada linha. Concluir resultado não conclui ações em cascata. O usuário escolhe para onde mover um resultado; não pressupor a existência de Algum dia/Talvez.
Datas comunicam o significado escolhido (compromisso, prazo, reconsideração). Estados vazios informam, sem incentivar preencher o espaço.
A revisão é pessoal e acontece ao examinar os registros. Não impor sessão, roteiro ou frequência obrigatória, nem avaliar a saúde do sistema. A recomendação semanal pode orientar convites futuros, distinguindo ausência de revisão registrada de ausência real de revisão. O roteiro fixo antigo foi retirado desta navegação; a experiência de revisão será desenhada na jornada correspondente.

## IA
Auxiliar, não decisora nem base da arquitetura. Pode organizar uma fala longa em proposta de listas/plano, apoiar clareza e revisão ou recuperar contexto. Propostas não são compromissos assumidos automaticamente. Não julgar um lembrete pela quantidade de detalhes. Perguntas e intervenções são opcionais e respeitam a resposta de manter algo como está. Hoje a assistência é demonstrativa e identificada, sem modelo conectado.

## Plataformas e processo
Mobile first, adaptado para tablet/desktop. Não confundir HTML responsivo com app nativo iPhone/iPad/Android. Guardar dados e relações na evolução e testar migrações. O código atual é protótipo local no navegador, sem sincronização.
Desenvolver primeiro; usuário vê e testa; só depois realizar teste simulado de usabilidade quando combinado. Verificações funcionais e visuais não são pesquisa com usuários. Agradecer feedback e reconhecer marcos com naturalidade; dar espaço à conversa sem executar automaticamente.

## Benchmark e alternativas de navegação
O usuário rejeitou o experimento de emoji em todas as listas. Restaurar a base vetorial sem apagar dados ou refazer a estrutura. Estudo visual separado em Estudo-navegacao.html compara três alternativas. O usuário escolheu aplicar A como próximo teste: ícones vetoriais próprios nas listas principais e um símbolo neutro comum nas sublistas, sem emojis. Consultar docs/BENCHMARK-NAVIGATION.md. Não copiar os ícones de progresso nem a taxonomia áreas/projetos de Things como hierarquia obrigatória.

## Proposta A aplicada
A diferenciação é visual e baseada na posição, sem alterar o modelo livre. O círculo das sublistas contém traços de lista e não preenchimento de progresso. O círculo de Things representa progresso de projetos; não usar esse significado para qualquer lista. Manter alinhamento, ritmo, pesos e divisórias da proposta.

## Teste atual: A com emojis nas principais
A pedido do usuário, testar emojis apenas nas listas principais, preservando o símbolo vetorial neutro das sublistas. Este teste substitui a orientação anterior de A inteiramente vetorial; não retorna aos emojis em todas as listas. Preservar alinhamento, pesos, divisórias e modelo livre. Emojis ficam associados à lista, estáveis ao renomear; sublistas não os exibem.

Hierarquia de peso: nome de lista principal sempre em seminegrito (600), com ou sem sublistas; nomes de sublistas em peso regular (400), inclusive quando selecionados. A posição define o peso, não o conteúdo.

## Decisão vigente: registros comuns, sem especialização de projeto
Esta decisão substitui as orientações anteriores sobre tipo projeto, conversão e vínculo projeto–ação. Projetos é uma lista comum; seus registros usam o mesmo editor, notas e checklist de qualquer item. Não há tela de projeto, contagem de ações relacionadas, conversão ou criação vinculada. Ações atuais ficam nas listas escolhidas pelo usuário; planejamento pode ficar nas notas. Campos legados kind/project são preservados inertes para evitar perda de dados antigos, sem efeitos na interface. Tags foram mapeadas no guia Things (pp. 16–17) como relação opcional, mas ficam para discussão futura, não implementadas. Antes de adicionar estrutura que interprete significado (tipos, inferências, vínculos, regras), avisar e combinar com o usuário. Não inferir projeto pela lista ou conteúdo.

Decisão visual vigente: encerrar o teste de emojis e restaurar ícones vetoriais nas principais, mantendo sublistas neutras e principais sempre em seminegrito. Próxima proposta deve tratar composição, busca, ritmo e estados em conjunto, sem adicionar semântica à estrutura.

## Revisão integrada da navegação
Ícones vetoriais, principais sempre em seminegrito, sublistas regulares com símbolo neutro de lista (sem círculo de progresso). Marca compacta; busca com superfície e atalho apenas em desktop. Ritmo por espaços entre grupos e divisórias apenas entre conjuntos com sublistas. Rodapé com Nova lista e controle explícito de ajustes; estado local disponível nos dados, sem mensagem permanente. Seleção, foco, toque e hover ajustados em claro/escuro. Preservar rolagem por lista e na navegação; transição curta respeita movimento reduzido. Nenhuma semântica de projeto adicionada.

Estudo de identidade separado em Estudo-identidade.html: A Presença (silhuetas preenchidas, contraste e acentos vivos), B Matéria (paleta mineral, traços abertos, ritmo mais amplo), C Horizonte (formas suaves, cores translúcidas e tons frios). Mesma estrutura e conteúdo demonstrativo, sem acesso ao storage. Comparação responsiva, claro/escuro, busca e abertura demonstrativa; não é pesquisa nem versão adotada. Aplicativo atual preservado até feedback.

Direção D Objetos acrescentada ao estudo por solicitação do usuário: referência Airbnb enviada, busca branca com sombra suave, fundo claro aquecido, ícones autorais ilustrados em SVG com luz, materiais e volume. Não são assets Airbnb nem emojis; estudo de linguagem, não produção de ícones fotorrealistas. A–C preservadas, app preservado. Usuário gostou mais de A mas considerou próxima demais de Things; C afasta-se da intenção desejada.

Direção D aprofundada em Direcao-D.html, sem alterar app/comparativo anterior. Três ícones vetoriais ilustrados refinados (bandeja, bússola como hipótese de próximas ações, ampulheta), luz/material comuns. Busca menos elevada, pesos tipográficos próximos, agrupamentos por ritmo. Controle demonstrativo de nomes longos/lista extensa e claro/escuro. Sem storage. Ícones restantes exploratórios; não alegar render 3D/fotorrealista.

Correção da direção D: a busca deve usar superfície escura no tema escuro, com texto/ícone claros e borda discreta; não manter a cápsula branca. Ajustado no comparativo e na prévia aprofundada.

Direção D, rodada 2 autorizada: quatro prioridades aplicadas na prévia Direcao-D.html. Linhas principais 46px, contextos 44px, título de grupo próximo dos filhos e pausa maior após conjunto; bússola simplificada e ampulheta mais larga; peso principal 520 e secundário 430; símbolos neutros com mais presença. Busca 48px, sombra reduzida, seleção com marca lateral e cor quente, em claro/escuro. App principal preservado.

Direção D rodada 3: títulos 600 e sublistas 400 para hierarquia estável, ritmo preservado. Bússola redesenhada com diâmetro maior e ponteiro mais simples, ampulheta com vidro e moldura mais largos, paleta dos materiais mais expressiva. Seleção apenas por superfície em claro/escuro, sem faixa ou mudança de cor do texto. Continua prévia separada. Renderização final deve ser julgada no dispositivo do usuário; screenshots locais não equivalem a iOS.

Família D redesenhada em conjunto: cinco objetos compartilham luz superior esquerda, inclinação de -5°, paleta de materiais e sombra de contato. Papel e coral reaparecem em bandeja/caderno, metal e coral na bússola, metal quente/vidro na ampulheta, verdes e cerâmica clara na planta. Mesma grade 32px, compensação por silhueta. Usuário reforçou que realismo é direção válida (referência Airbnb), não tratar volume/ilustração como defeito; julgar execução e consistência. Restante da tela preservado.

## Identidade principal aprovada: direção D
Usuário celebrou a identidade própria e autorizou promover D ao aplicativo principal. Esta decisão substitui os testes A/emojis/estudos anteriores. Clareza.html usa família ilustrada autoral D (cinco objetos e papel neutro para listas livres), busca tátil, paleta quente, títulos 600/sublistas 400, ritmo compacto e seleção por superfície. Sublistas permanecem neutras. Sem marca no topo; fechamento mobile preservado. Mesma família em títulos/seletores/busca e organização. Captura, edição, organização, armazenamento e modelo livre preservados; nenhuma nova semântica de projeto. Direcao-D.html continua como estudo histórico.

Auditoria de consistência D: corrigidas superfícies e cores legadas em captura/editor, datas, seletores, busca, listas, organização, ajustes e assistência demonstrativa. Base quente por tokens canvas/surface/field, texto/apoio, bordas, acento e foco; diálogos com leve transição quente, sem azul legado ativo nesses componentes. Fonte de sistema herdada e ritmo 8/16/24; campos mobile 16px, alvos principais >=44px. Sem redesenho de jornada ou mudança nos dados. Meta theme-color por tema.

Setup mobile: usuário explicitou que revisões devem avaliar experiência/jornada, objetivos, descobribilidade, fricções e oportunidades; verificação técnica apoia, não substitui, avaliação de usabilidade. Distinguir revisão especializada de evidência com participantes reais. Cinco correções autorizadas: seletor de localização fecha para formulário preservado por ×/Escape/Voltar, busca de localização com caminho e tolerância a acentos, reordenação preserva rolagem e foco no controle usado (fallback no limite), Lista aqui com alvo >=44px e texto legível, setas com acento D sem azul legado. Nenhuma alteração na semântica de listas.

Protótipo de espaços em Espacos.html, separado do principal e da chave de dados real; usa clareza.spaces-study.v1 com dados demonstrativos. Inbox universal, Pessoal/Profissional com listas livres independentes, seletor fixo no rodapé e gesto horizontal complementar. Destinos mostram caminho completo, mover lista preserva subárvore, novos espaços podem copiar estrutura sem registros. Referência Arc para orientação e transição, mantendo identidade D. Não tratar o estudo como recurso lançado no app principal.

Espaços opção 2 em Espacos-2.html, separado do principal e da opção 1, dados clareza.spaces-study.v2. Usuário rejeitou seletor distante no rodapé; confirmou espaço como universo de atenção, com 2–3 mais comuns mas quantidade livre. Busca e Inbox universais fixas; nome do espaço é o próprio controle discreto entre Inbox e listas. Menu ancorado com nomes completos, seleção atual e busca quando >5; gestão secundária. Sem tabs no rodapé ou swipe nesta hipótese. Listas mantêm composição D; movimento entre espaços preservado. Só um espaço: título sem controle desnecessário.

Estudo Espacos-movimento.html: usuário rejeitou dropdown e faixa de tabs; pediu bolinhas discretas, gesto e visão geral como mesas do macOS. Estudo sem storage: busca/Inbox fixas, listas em scroll horizontal nativo com snap e rolagem vertical própria, posição por até 5 indicadores + fração quando muitos, visão geral na região das listas com miniaturas reais e criação de espaços sem registros copiados. Preserva memória de lista/rolagem por ambiente. Mouse e teclado complementam toque. Nenhuma mudança no app principal.

Refinamento autorizado do estudo de movimento: remover ícone junto ao nome (título continua tocável; acesso explícito único no rodapé), indicadores logo após a superfície de listas dimensionada pelo conteúdo e limitada à altura disponível. Até cinco espaços: bolinhas estáveis; mais: contador n/total tocável abre visão geral, sem janela de bolinhas mudando de posição. Controle de lista extensa para conferir gestos horizontal/vertical. App principal preservado. Testes em Chromium não substituem Safari/iPhone físico.

Estudo Espacos-navegacao.html corrige a separação entre navegação e conteúdo: carousel/bolinhas/visão geral apenas no sidebar; clicar em lista abre main à direita ou fecha navegação mobile. Trocar espaço atualiza também main para última lista válida daquele ambiente, ou primeira raiz existente, ou visão vazia. Inbox universal; trocar espaço a partir dela também abre lista do destino. Chave separada clareza.spaces-study.v3, dados demonstrativos. Mantidos editores e mover entre espaços. App principal preservado.

Estudo de abrangência em Espacos-ambiente.html: camada global de busca/Inbox fora de uma moldura de ambiente que engloba navegação e conteúdo, título compartilhado e superfícies sutis coerentes nos dois lados. Visão geral cobre toda essa moldura e prévias mostram navegação+conteúdo. Gesto continua na navegação com resposta coordenada discreta no main. Mantém última lista por ambiente; chave separada v4 e dados de demonstração, sem alterar principal.

## Captura refinada autorizada
Título em foco, nota discreta sempre disponível e data/tags/checklist progressivos na identidade D. Enter no título guarda (Shift+Enter nova linha); Enter na nota cria linha; Tab navega sem guardar. Botão Guardar e alternativa Guardar e continuar. Captura também no rodapé do menu. Rascunho mantém texto, destino, notas, tags, checklist e data em chave separada clareza.prototype.v1.captureDraft; ao reabrir mantém DOM/cursor e histórico recente de até 60 estados de escrita nesta aba. Ctrl/Cmd+Z e redo no compositor; histórico não promete recuperar clipboard do sistema nem sobreviver a recarga (rascunho atual sobrevive). Captura só confirma sucesso após persistência; no erro desfaz inclusão em memória e mantém rascunho aberto. Tokens evitam recuperar como rascunho uma captura já guardada caso limpeza falhe. save retorna booleano; criação inline não prossegue após falha. Busca global e destinos normalizam acentos, palavras incompletas e erros curtos; “aCOIS” encontra Próximas ações. Tags são metadados livres opcionais, editáveis no registro e pesquisáveis, sem relações ou classificação automática de projetos. Espaços seguem adiados, principal sem espaços.

Captura: removida a instrução textual de teclado sob o compositor a pedido do usuário; interação deve ser intuitiva. Atalhos preservados.

Captura: removidos o texto de atalhos e o botão secundário Guardar e continuar a pedido do usuário. Apenas Guardar permanece como ação visível de gravação.

Editor de registros alinhado à captura: mesma superfície, título/nota, ferramentas de data/tags/checklist e destino no rodapé. Conclusão ao lado do título; assistência e exclusão em Mais opções. Sem texto permanente de autosave. Edição mantém gravação automática; Pronto/Enter no título confirma e fecha.

## Microinterações como princípio
Todas as ações devem ter uma resposta perceptível, clara e proporcional: estado de pressão, transição de contexto ou confirmação de resultado. Movimento deve explicar a ação, nunca atrasar a interação, exigir espera ou virar decoração. Respeitar movimento reduzido, teclado, toque e temas claro/escuro. Aplicar progressivamente a cada jornada; não afirmar que todas as ações já foram revisadas.
Primeira rodada: + global/menu responde à pressão e abre captura com elevação curta (230ms); tocar uma tarefa responde à pressão e revela editor com expansão discreta (210ms). Fundo acompanha em 180ms. Campos recebem foco imediatamente, sem esperar animação; rascunhos e persistência preservados.
