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
- Things é referência de cuidado visual, não copiar marca/Inbox. Iconografia própria (emojis únicos no experimento atual); tipografia, espaçamento, alinhamento e comportamento consistentes; sem breadcrumb; temas claro/escuro completos.
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

## Experimento visual mais recente
Usuário autorizou trocar os ícones de listas/sublistas por emojis únicos, mantendo a composição atual de hierarquia. A preferência anterior por ícones vetoriais preenchidos para listas foi substituída para este teste visual. Emojis são atribuídos e preservados por lista, não impostos pelo significado do método. Não alterar estrutura ou fluxos por causa desse teste.
