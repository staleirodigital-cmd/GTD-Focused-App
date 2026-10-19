# Orientações do projeto

Leia PROJECT_CONTEXT.md e DESIGN.md antes de alterar produto/interface. Ambos registram o entendimento mais recente; os agrupamentos fixos de versões antigas foram explicitamente revogados. Consulte docs/GTD-REFERENCES.md para a base metodológica.

- Listas reais, independentes ou aninhadas; template totalmente editável/removível. Não voltar a categorias obrigatórias nem inferir significado pelo nome/localização.
- Captura global inicia na Inbox, mas permite qualquer lista e criação inline preservando o rascunho. Não voltar a Inbox obrigatória.
- Hierarquia visual por composição, sem recuos em cascata. Refinamento, divulgação progressiva, toque/teclado e contraste são essenciais.
- A pessoa julga a confiabilidade. IA e revisão não diagnosticam qualidade por texto, idade ou ausência de próxima ação.
- Clareza.html é a fonte independente entregue. Preservar a chave de storage clareza.prototype.v1 e a migração para payload v2. Não executar scripts antigos de patch/reconstrução: eles representam estados históricos.
- Execute npm test para verificações de dados/sintaxe. Regressões de navegador são técnicas e não pesquisa com usuário. Usuário vê/testa antes de qualquer nova simulação de usabilidade, conforme combinado.
- Agradecer feedback e reconhecer marcos com naturalidade. Quando o usuário quer conversar ou dar feedback, não iniciar alterações automaticamente.
- Manter memória e guias de projeto versionados; não publicar PDFs integrais/extrações no repositório público. Não alegar que arquivos locais são memória permanentemente disponível.

## Teste atual: A com emojis nas principais
A pedido do usuário, testar emojis apenas nas listas principais, preservando o símbolo vetorial neutro das sublistas. Este teste substitui a orientação anterior de A inteiramente vetorial; não retorna aos emojis em todas as listas. Preservar alinhamento, pesos, divisórias e modelo livre. Emojis ficam associados à lista, estáveis ao renomear; sublistas não os exibem.

## Decisão vigente: registros comuns, sem especialização de projeto
Esta decisão substitui as orientações anteriores sobre tipo projeto, conversão e vínculo projeto–ação. Projetos é uma lista comum; seus registros usam o mesmo editor, notas e checklist de qualquer item. Não há tela de projeto, contagem de ações relacionadas, conversão ou criação vinculada. Ações atuais ficam nas listas escolhidas pelo usuário; planejamento pode ficar nas notas. Campos legados kind/project são preservados inertes para evitar perda de dados antigos, sem efeitos na interface. Tags foram mapeadas no guia Things (pp. 16–17) como relação opcional, mas ficam para discussão futura, não implementadas. Antes de adicionar estrutura que interprete significado (tipos, inferências, vínculos, regras), avisar e combinar com o usuário. Não inferir projeto pela lista ou conteúdo.

## Revisão integrada da navegação
Ícones vetoriais, principais sempre em seminegrito, sublistas regulares com símbolo neutro de lista (sem círculo de progresso). Marca compacta; busca com superfície e atalho apenas em desktop. Ritmo por espaços entre grupos e divisórias apenas entre conjuntos com sublistas. Rodapé com Nova lista e controle explícito de ajustes; estado local disponível nos dados, sem mensagem permanente. Seleção, foco, toque e hover ajustados em claro/escuro. Preservar rolagem por lista e na navegação; transição curta respeita movimento reduzido. Nenhuma semântica de projeto adicionada.

## Identidade principal aprovada: direção D
Usuário celebrou a identidade própria e autorizou promover D ao aplicativo principal. Esta decisão substitui os testes A/emojis/estudos anteriores. Clareza.html usa família ilustrada autoral D (cinco objetos e papel neutro para listas livres), busca tátil, paleta quente, títulos 600/sublistas 400, ritmo compacto e seleção por superfície. Sublistas permanecem neutras. Sem marca no topo; fechamento mobile preservado. Mesma família em títulos/seletores/busca e organização. Captura, edição, organização, armazenamento e modelo livre preservados; nenhuma nova semântica de projeto. Direcao-D.html continua como estudo histórico.
