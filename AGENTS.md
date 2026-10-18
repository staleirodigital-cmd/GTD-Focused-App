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
