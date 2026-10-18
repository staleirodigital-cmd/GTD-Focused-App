# Clareza · GTD Focused App

Um espaço pessoal para listas, lembretes e projetos, inspirado no GTD. A organização inicial é um template: você pode mudar o nome, mover e remover qualquer lista sugerida.

[Abrir o protótipo](https://staleirodigital-cmd.github.io/GTD-Focused-App/Clareza.html)

## Usar localmente
Abra `Clareza.html` no navegador, sem instalação ou dependências externas. Para servir por HTTP: `python3 -m http.server 4173`, depois abra `http://localhost:4173/Clareza.html`.

## O que funciona
- Captura rápida com Inbox como destino inicial editável. Busca de destino e criação de lista no mesmo fluxo, sem perder o texto.
- Listas independentes e listas dentro de listas. Abrir o conjunto ou o recorte usa os mesmos registros, sem duplicação.
- Nome e localização editáveis; ordenação, movimentação e remoção com preservação de conteúdo e desfazer.
- Arrastar no desktop: centro para inserir dentro; bordas superior/inferior para ordenar. As opções de localização e os botões de ordem são alternativas explícitas para toque e teclado.
- Hierarquia visual por conjuntos alinhados, sem árvore de recuos. Mobile first, adaptado para tablet/desktop, claro e escuro.
- Notas, checklists embutidos e apresentação opcional de lista como checklist. Conferir um item de checklist não o conclui como compromisso.
- Transformação explícita de item em projeto e relações projeto-ação, sem depender da lista onde estão. Mover para Projetos não transforma automaticamente um item.
- Busca, datas com significado explícito, conclusão, exportação e importação JSON.
- Assistência demonstrativa identificada, sem modelo de IA conectado.

## Dados e migração
Os dados ficam neste navegador, sem sincronização. A chave `clareza.prototype.v1` foi mantida e o conteúdo passou para versão 2. A migração mantém IDs e relações e guarda uma cópia bruta anterior em `clareza.prototype.v1.before-v2`. Listas removidas não reaparecem. Exporte cópias dos seus dados. Remover uma lista preserva itens e sublistas: conteúdo sobe ao pai; na raiz, itens vão para Inbox e sublistas ficam em Meu espaço.

## Desenvolvimento
`npm test` executa verificações sem dependências: sintaxe, agregação genérica, intenção explícita, listas livres, exclusão sem perda, ciclos e migração/backup. Os testes de navegador em `tests/free-lists-*.cjs` são regressões técnicas opcionais com Playwright e Chromium; não constituem validação de usabilidade. Use `CHROMIUM_PATH` para indicar um executável instalado ou instale o Chromium do Playwright.

Leia [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md), [DESIGN.md](DESIGN.md) e [a síntese das referências](docs/GTD-REFERENCES.md). As decisões recentes substituem o modelo inicial de categorias fixas.

## Limites
Não há conta, sincronização, notificações ou integração com calendário. O HTML responsivo não é um aplicativo nativo iOS/iPadOS/Android. O roteiro fixo antigo de revisão foi retirado; a experiência de revisão será desenhada no contexto da jornada, sem exigir sessão ou declarar a saúde do sistema. A primeira avaliação de uso desta versão será do usuário antes de uma nova simulação.

Dados inseridos no navegador não são enviados ao repositório. Os PDFs integrais de referência não estão incluídos no repositório público; a documentação contém sínteses próprias.
