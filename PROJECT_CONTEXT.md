# Contexto permanente · Clareza / GTD Focused App

## Como retomar
Leia este arquivo, AGENTS.md e DESIGN.md antes de agir. Não peça novamente ao usuário os conceitos já acordados. O repositório é https://github.com/staleirodigital-cmd/GTD-Focused-App (main). O protótipo independente é Clareza.html. O Pages está em https://staleirodigital-cmd.github.io/GTD-Focused-App/Clareza.html. Confira a publicação efetiva antes de dizer que uma mudança está disponível.

## Intenção e fundamentos acordados
Criar um sistema pessoal inspirado no GTD, com o cuidado e fluidez de Things, Apple, Nubank e Airbnb. Things é referência de refinamento, não modelo a copiar nem estrutura obrigatória. O guia GTD de 2018 usa recursos de Things como recipientes para listas próprias; nosso produto deve representar essa intenção diretamente.
Uma captura é uma coisa que tem atenção. O usuário define significado e intenção. Uma ação resolve um compromisso em um passo; um projeto representa um resultado que exige mais de uma ação, mesmo pequeno. Pode haver apenas uma próxima ação conhecida. Não contar checklist para inferir projeto. Lista é organização para uma finalidade e não vira projeto por conter itens.
Agrupamentos Próximas ações, Projetos, Aguardando, Algum dia/Talvez e Referência são clicáveis. Contextos (Na rua, Em casa, No telefone, No computador, pessoas/reuniões) são listas dentro de Próximas ações. O agrupamento reúne registros; abrir contexto filtra sem cópia. Sublistas devem permitir organizar pessoas, equipes e outros recortes; o significado é herdado do agrupamento. Uma lista pode conter itens e sublistas. Não diferenciar listas oficiais de suas listas.
Projetos abrem visão própria do resultado, suporte e ações relacionadas; edição nos detalhes. Ações aparecem no contexto e no projeto mantendo uma identidade. Esperas e possibilidades não poluem próximas ações.

## UX acordada
Mobile first, adaptado para tablet/desktop e preparado conceitualmente para futura base iOS/iPadOS/Android. HTML responsivo não é app nativo. Divulgação progressiva: lista mostra títulos/indicadores; nota aparece ao examinar item; operações revelam opções quando necessário. Sem breadcrumb. Ícones preenchidos, coerentes e originais (não copiar Inbox do Things). Refinamento por tipografia, ritmo, proporção e comportamento, não decoração. Não adicionar telas/burocracia para demonstrar metodologia. Contraste e consistência em claro/escuro.
Uma criação Nova lista global; operações contextuais nas opções, sem vários + permanentes. Agrupamentos claramente clicáveis, contextos recuados e legíveis, sem recolhimento prematuro. Alvos de toque e foco visível.
Captura global + e N sempre Inbox. Adicionar próxima ação é contextual e vincula projeto. Não repetir nome do projeto dentro do próprio projeto. Datas mostram seu significado (compromisso/prazo/reconsideração). Acompanhamento cria ação escrita pelo usuário e preserva espera. Concluir projeto não conclui ações em cascata. Reconsiderar depois move resultado, informa preservação de ações.

## IA
Apoiar clareza e revisão, não presumir contexto ou compromisso. Exemplo carro: pessoa pode já ter agendado, entregue, ou estar avaliando troca; não gerar telefonema/plano com base apenas na anotação. Assistência opcional, sem entrevista/bloqueio. Gestos como renomear/mover podem esclarecer. Hoje assistência é demonstrativa e identificada; sem modelo conectado.

## Estado e verificação anteriores
Arquivo independente HTML/CSS/JS com localStorage clareza.prototype.v1, export/import JSON, migração, projetos, notas, checklist, busca, datas, revisão inicial. Sem conta, sync, notificações nem integração calendário. Fonte principal contém JS em script type module e CSS embutido.
Já houve teste simulado de captura durante projeto, ação na rua e espera. Problemas corrigidos: captura contextual indevida, significado de datas, repetição de projeto, conclusão/reconsideração, estados vazios. Código publicado no commit 69f8555bac931131add5fb8e897c77ab185feb84 antes desta etapa. Arquivos temporários de testes podem conter seletores/comportamentos antigos; não tratá-los como especificação.

## Etapa atual e sequência explícita do usuário
Desenvolver primeiro a jornada de setup/adaptação de listas e sublistas com cabeça de staff product designer, simplicidade, experiência e jobs do usuário. Objetivos: começar sem configuração obrigatória; adicionar contexto; criar Assuntos a tratar > Ana; renomear; mover/reordenar/remover listas preservando conteúdo.
Depois de ver o primeiro resultado, o usuário fará seu próprio teste. Só depois discutir teste simulado. NÃO rodar agora teste simulado de usabilidade nem apresentar hipótese como pesquisa com usuário. Verificações técnicas (integridade, sintaxe, renderização) continuam necessárias.

## Colaboração
Agradecer feedback, reconhecer conquistas e celebrar marcos com naturalidade. Não executar automaticamente quando usuário quer conversar ou dar feedback. Escutar e alinhar antes de novas alterações nessas situações. Não repetir confirmações já autorizadas.

## Memória e arquivos
Este documento e DESIGN.md/AGENTS.md devem acompanhar o código no GitHub para sobreviver à troca de ambiente. Arquivos locais sozinhos podem se perder numa reinicialização; não prometer memória ilimitada ou persistência de /workspace. Guias originais guardados em /workspace/reference/gtd/originals, textos em /workspace/reference/gtd/text e índice com SHA-256 em /workspace/reference/gtd/index.json. Pacote de recuperação: /workspace/Clareza-guias-de-referencia.zip. Não incluir PDFs ou transcrições integrais no repositório público; manter referência e síntese próprias em docs/GTD-REFERENCES.md.

## Implementação da etapa de setup
Listas agora têm parent; group é mantido para compatibilidade e derivado do ancestral. Agregações percorrem descendentes sem cópia. Criar lista tem nome e localização sob demanda; Criar sublista pré-preenche pai atual. Opções permitem renomear, mover estrutura, reordenar irmãos e remover sem apagar itens/sublistas (realoca no pai). Migração idempotente preserva dados e importação rejeita ciclos. Novo seed tem quatro contextos e zero tarefas; convite inicial é opcional. Organizar listas está nas opções da Inbox/grupos e opções/dados. Modelo e renderização foram conferidos tecnicamente; NÃO foi feita nova simulação de usabilidade. Próximo passo: usuário vê o resultado e faz seu próprio teste; aguardar feedback.
