# Clareza · GTD Focused App

Protótipo de um sistema pessoal inspirado no Getting Things Done, com listas flexíveis, contextos e divulgação progressiva. Mobile first, com adaptação para tablet e desktop.

## Experimentar

Abra **Clareza.html** no navegador. O arquivo é independente e não exige instalação nem dependências externas.

Para servir localmente, execute `python3 -m http.server 4173` na raiz e abra `http://localhost:4173/Clareza.html`.

## Experiência atual

- Captura imediata, edição, conclusão e desfazer.
- Próximas ações como visão geral agrupada por contextos; abrir um contexto filtra os mesmos registros, sem duplicação.
- Agrupamentos de Projetos, Aguardando, Algum dia/Talvez e Referência, com criação e reclassificação de listas.
- Projetos com notas, checklists e ações relacionadas acessíveis também nos contextos.
- Busca, datas com significado explícito e roteiro inicial de revisão.
- Dados no navegador, exportação/importação JSON e migração dos registros do protótipo anterior.
- Assistência de esclarecimento demonstrativa, identificada na interface. Nenhum modelo de IA está conectado.

## Princípios

Leia [DESIGN.md](DESIGN.md) antes de alterar o produto. O objetivo é oferecer a liberdade do papel com uma interface refinada, sem burocratizar o GTD. A IA ajuda a esclarecer; contexto, intenção e compromisso pertencem ao usuário.

## Verificação

Com Node.js instalado, execute `npm test` (sem instalar dependências). O teste verifica a sintaxe do aplicativo e a lógica de agregação, contextos, exclusão de itens não executáveis, migração e reclassificação.

A conferência visual completa no preview continua pendente. As verificações de dados não substituem testes de usabilidade e acessibilidade.

## Limites do protótipo

Os dados ficam no armazenamento local do navegador; não há conta ou sincronização. Faça exportações para manter cópias. Datas não geram notificações. A revisão não lê calendários nem materiais externos. O HTML atual não é um aplicativo nativo para iPhone, iPad ou Android; essa arquitetura será definida na evolução do produto.

Os dados de exemplo fazem parte do código. Registros inseridos pelo usuário no navegador não são enviados ao repositório. Os PDFs de referência não estão incluídos.
