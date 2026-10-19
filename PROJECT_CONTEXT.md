# Memória versionada do projeto · Clareza

## Retomada
Ler AGENTS.md, DESIGN.md e este arquivo antes de mudanças. Repositório: https://github.com/staleirodigital-cmd/GTD-Focused-App (main). Pages: https://staleirodigital-cmd.github.io/GTD-Focused-App/Clareza.html. Confirmar a versão publicada antes de entregar o link. Clareza.html é a fonte executável independente atual.

## Objetivo e entendimento consolidado
Um espaço pessoal para praticar GTD com liberdade e refinamento comparável ao Things. O coração é o apoio ao fluxo de capturar, esclarecer, organizar, engajar e revisar, sem impor etapas obrigatórias da interface. A organização é meio; quem julga a confiança é a pessoa. Não marcar itens/projetos como errados por idade, texto curto ou falta de próxima ação.
Usuário voltou deliberadamente à discussão estratégica porque nossa implementação tinha virado categorias fixas e um app de tarefas. O guia GTD para Things ignora parte da arquitetura nativa e constrói listas próprias sobre recursos do software. O princípio a incorporar é liberdade real para construir o sistema, não apenas flexibilidade dentro de categorias fixas.

## Decisões vigentes (substituem as primeiras versões)
- Listas e sublistas são a mesma entidade, com posição editável. Podem ter itens e listas filhas. Listas independentes ficam em Meu espaço.
- O template inicial é comum, não obrigatório. É possível renomear, mover e apagar também Projetos, Próximas ações, Aguardando, Algum dia/Talvez. Não recriar listas apagadas nem preservar uma taxonomia oculta.
- Abrir lista-pai reúne seus registros e descendentes sem duplicação. Nenhuma semântica de compromisso é inferida pelo nome/destino.
- Um projeto é resultado com mais de uma ação requerida, mesmo pequeno. Transformação explícita, conteúdo preservado; relação projeto-ação independente da árvore. Checklist não define projeto.
- Inbox é o destino inicial da captura global, mas o seletor permite qualquer lista e criação inline. A orientação anterior de Inbox obrigatória foi revogada. Adicionar aqui mantém o contexto; relacionar ação a projeto é explícito.
- Nova lista está disponível; não usar convite alto, tour, questionário ou tarefas fictícias. Nome e localização; Criar lista aqui pré-preenche pai. Encaminhar item deve permitir criar destino sem perder rascunho, inclusive no cancelamento.
- Arrastar permite reorganização direta no desktop, com indicação antes/depois/dentro e proteção contra ciclos. Mover pelas opções e ordenar por botões são alternativas disponíveis.
- UI: hierarquia por agrupamento, peso, espaço e divisórias; linhas alinhadas. NÃO usar recuos em cascata. Estruturas profundas são exploradas abrindo as listas.
- Things é referência de cuidado visual, não copiar marca/Inbox. Iconografia vetorial própria; tipografia, espaçamento, alinhamento e comportamento consistentes; sem breadcrumb; temas claro/escuro completos.
- Ao abrir item, mostrar detalhes necessários. Na lista, só título/indicadores. Notas vazias não ocupam espaço até solicitadas.
- Revisão pessoal, sem seção obrigatória ou roteiro julgando o sistema. Cadência semanal é recomendação, pode gerar convite futuro; ausência de registro não prova ausência de revisão. Respeitar ritmo e decisão de deixar projeto sem ação.
- IA é auxiliar e pode surgir naturalmente nas jornadas. Pode estruturar discurso em proposta de plano/listas, apoiar clareza e questionar sem diagnosticar. Ex.: carro pode já estar agendado/entregue, não inventar telefonema. Texto curto pode ser suficientemente esclarecido. Propostas precisam ser distinguíveis de compromissos do usuário.

## Implementação atual
Fonte HTML/CSS/JS independente; storage key clareza.prototype.v1 é preservada, mas payload agora usa version:2. Listas reais {id,name,parent,icon,format?}, sem group/categorias obrigatórias. Inbox é destino de captura e permanece como recipiente básico; Meu espaço e Concluídos são recursos de navegação, não listas de compromisso.
Migração v1 materializa antigos agrupamentos implícitos, mantém IDs, notas, checklists, relações e conteúdo, salva cópia bruta em clareza.prototype.v1.before-v2. v2 não recria listas removidas. Import rejeita ciclos e referências inválidas; se dados não puderem ser lidos, os originais são preservados e gravação é bloqueada até recuperação/importação.
Navegação mostra raízes e seus filhos imediatos com composição alinhada. Profundidade maior fica dentro da página de lista. Criação independente/contextual, edição de nome/localização, exclusão sem perda, ordenação e drag/drop. Seletor de destino compartilhado por captura e mover, com busca e criação inline preservando rascunho. Captura usa destino editável, sem inferir projeto. Checklists podem ser apresentação opcional de lista, com checked separado de done; checklist embutido continua.
Projetos: visão própria com suporte e registros relacionados nas listas reais, conclusão explícita sem cascata, mover para qualquer lista. Roteiro fixo de revisão removido da navegação; a jornada correspondente será trabalhada depois. IA continua demonstrativa e identificada; não há modelo conectado.
Sem conta, sincronização, notificações, calendário ou apps nativos. Dados permanecem no navegador, export/import JSON. Não alegar essas capacidades prontas.

## Estado do trabalho e próxima conversa
Usuário autorizou implementar a jornada livre e contextual com a referência visual enviada. Fazer verificações técnicas, não nova pesquisa/teste simulado de usabilidade. Próximo passo é ele ver e experimentar o resultado, compartilhar feedback e só então discutir simulação. Não avançar em IA/revisão/arquitetura nativa sem necessidade da jornada.
Model checks e regressões funcionais cobrem criação independente, agregação, remoção de antigos agrupamentos, migração, preservação de texto na criação inline, drag/drop e conferência separada de conclusão. Não são evidência de validação com usuários.

## Processo humano
Agradecer feedback positivo, reconhecer conquistas e comemorar marcos com naturalidade. Não ser apenas execução automática. Quando usuário pede espaço para feedback, ouvir e alinhar antes de alterar. Evitar pedir novamente decisões consolidadas.

## Fontes e recuperação
Referência Things: https://culturedcode.com/things/support/. Guias locais em /workspace/reference/gtd/originals, textos em /workspace/reference/gtd/text, índice com SHA-256 em /workspace/reference/gtd/index.json. Síntese própria rastreável em docs/GTD-REFERENCES.md. Pacote privado de recuperação: /workspace/Clareza-projeto-e-referencias.zip. PDFs integrais/transcrições não são publicados no repositório público. Documentação no GitHub sobrevive à troca de ambiente; não prometer persistência ilimitada de /workspace ou memória fora destes arquivos.

## Feedback visual mais recente
O usuário rejeitou os emojis em todas as listas e pediu removê-los. Base vetorial restaurada, preservando modelo livre e dados. Pediu benchmark com Things e três formas visuais de distinguir listas e sublistas sem copiar sua taxonomia. Estudo separado em Estudo-navegacao.html para comparar: A ícones próprios nas principais e símbolo neutro nas sublistas; B símbolos estruturais de coleção/lista; C hierarquia tipográfica sem ícones nas sublistas. Ainda não há escolha definitiva. Benchmark no print fornecido e documentação oficial, não teste de usabilidade com participantes.

## Escolha mais recente
Usuário escolheu aplicar a proposta A do estudo, com ícones vetoriais em vez de emojis. Listas principais mantêm identidade própria; sublistas usam um símbolo neutro comum, circular com traços internos. Preservar composição, modelo livre e fluxos. Usuário explicou que o círculo preenchido de Things comunica proporção de tarefas concluídas; não confundir esse indicador de progresso com posição hierárquica. Nenhum preenchimento foi implementado neste teste.

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
