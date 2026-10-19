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
