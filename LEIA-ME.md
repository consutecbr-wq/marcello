# Site profissional de Marcello — revisão de 05/10/2026

## Abrir a versão revisada

Abra `index.html` com Chrome, Edge ou Firefox. O site funciona diretamente da pasta, sem instalação, compilação, JavaScript ou serviços de fontes e imagens externas.

O botão “Baixar resumo profissional” aponta para `assets/marcello-resumo-profissional.pdf`, um documento A4 de duas páginas. Dependendo do navegador, o PDF pode abrir em uma aba em vez de ser baixado automaticamente; nesse caso, use a opção de download do leitor.

A página `resumo-profissional.html` oferece o mesmo resumo em HTML para leitura e impressão. Use a opção Imprimir do navegador (Ctrl+P) para imprimir ou salvar em PDF. O PDF fornecido foi diagramado e verificado separadamente; a paginação da impressão do HTML pode variar conforme o navegador e suas configurações.

## Arquivos da pasta publicada

- `index.html`: apresentação principal, dois casos visíveis, trajetória resumida e contatos.
- `assets/styles.css`: estilos consolidados, foco, contraste, composição responsiva e impressão da página principal.
- `assets/marcello.png`: retrato original, preservado.
- `assets/ambiente-ilustrativo.webp`: imagem original de cozinha criada com IA, em posição secundária e identificada como ilustrativa.
- `assets/favicon.svg`: favicon com as iniciais MG.
- `assets/marcello-resumo-profissional.pdf`: resumo profissional de duas páginas, com contatos clicáveis.
- `resumo-profissional.html`: versão do resumo para leitura e impressão.
- `assets/resumo.css`: estilos de tela e impressão do resumo.
- `.nojekyll`: arquivo auxiliar de hospedagem estática, preservado.
- `LEIA-ME.md`: documentação da entrega.

## Contatos implementados

- E-mail: `mailto:consutecbr@gmail.com`.
- WhatsApp: `https://wa.me/5543991167868` (+55 43 99116-7868).
- LinkedIn: `https://www.linkedin.com/in/marcellogf/`.

E-mail depende de aplicativo ou serviço configurado no dispositivo; WhatsApp e LinkedIn dependem de conexão. Não há formulário, rastreamento ou coleta de dados implementados. Nenhuma mensagem foi enviada nos testes.

## Conteúdo e limites editoriais

Fonte: instruções confirmadas do usuário para esta revisão e arquivos locais inspecionados. Não havia currículo na pasta; o documento gerado é um “Resumo profissional”, uma seleção de experiências, e não um currículo completo.

- A abertura apresenta nome, foco em pós-venda e apoio técnico-operacional, contribuição, Londrina/PR e WhatsApp.
- Os casos VOI e Sensormatic/Kognos exibem informações essenciais sem blocos recolhidos. As duas últimas empresas têm períodos e posições distintos na trajetória.
- O esquema de especificação, pedido, alteração e conferência é uma representação ilustrativa do fluxo; não simula um documento original da VOI.
- Compras técnicas, desenhos, pedidos, fornecedores e acompanhamento recebem destaque. Autorizações de pagamento são descritas conforme as condições acordadas, sem afirmar execução bancária.
- TopSolid Design, dois meses trabalhando com montadores e aprendizado e operação de CNC durante 30 dias constam como vivências. Não foram atribuídos programação CNC, manutenção especializada, supervisão de montagem, 5S ou PCP.
- VOI: início em fevereiro de 2025; fechamento principal em junho de 2026; serviços adicionais de informática em julho e agosto de 2026. A data formal de término do vínculo regular permanece explicitamente não confirmada.
- Kognos Tecnologia: consultor sênior em negócio próprio, junho de 2012 a dezembro de 2017.
- Sensormatic: consultor sênior, outubro de 2006 a maio de 2012.
- Microsens: gerente técnico-comercial de licitações, janeiro de 1994 a março de 2003. A diretoria fechava as compras.
- Casa do Cliente aparece como ideia apresentada, não implantada, cujo detalhamento aguardava aprovação de diretrizes e prioridades. Não foram acrescentadas afirmações de implantação de ERP.
- Não foram acrescentados resultados numéricos, clientes identificados da Kognos, depoimentos, gestão de franquias ou dados privados de saúde, finanças, família e conflitos internos.

## Metadados e compartilhamento

Título, descrição, idioma e favicon estão definidos. A página principal inclui Open Graph com título, descrição, tipo, idioma, nome e URL pública.

A URL `https://consutecbr-wq.github.io/marcello/` respondeu HTTP 200 na revisão. Não foi declarado `og:image`: o retrato não estava disponível em `https://consutecbr-wq.github.io/marcello/assets/marcello.png`. Os metadados não dependem de uma imagem remota inexistente. Após uma publicação futura e a verificação do endereço da imagem, esse campo pode ser acrescentado.

## Verificações realizadas

- Integridade dos caminhos relativos de HTML, CSS, favicon, imagens e PDF, inclusive resolução sob `/marcello/`.
- Destinos das âncoras internas, IDs únicos, referências ARIA, idioma e um título principal por página.
- E-mail, LinkedIn e WhatsApp conferidos no HTML principal, no resumo em HTML e nos hyperlinks do PDF.
- Conteúdo dos casos visível no HTML sem JavaScript ou interação; nenhum placeholder ou recurso externo de interface incluído.
- Dimensões declaradas das imagens correspondem aos arquivos; ambos os originais foram preservados por comparação SHA-256 com a cópia de segurança.
- Cálculo das combinações de cores de texto usadas: todas superam 4,5:1; a menor combinação calculada é aproximadamente 5,35:1. Isso verifica contraste de texto, não certifica conformidade WCAG integral.
- CSS com blocos balanceados, regras de foco e movimento reduzido, limites de largura de texto e regras responsivas. Esta checagem estrutural não substitui renderização no navegador.
- PDF A4 de duas páginas aberto, extraído, renderizado com Poppler e inspecionado visualmente. Períodos, limites das funções e contatos conferidos.

## Verificações visuais pendentes

A ferramenta de navegador bloqueou a abertura local por protocolo `file:` na avaliação anterior. Esse bloqueio não foi contornado. A página HTML revisada não teve validação visual concluída.

Ainda é necessário abrir a versão revisada em um navegador e conferir 360, 768 e 1440 pixels, zoom de 200%, ausência de rolagem horizontal e recortes, imagens carregadas, navegação por teclado e indicação de foco. As regras responsivas estão implementadas, mas esses comportamentos não foram declarados como visualmente testados.

## Backup e ferramentas de autoria

Uma cópia completa da versão anterior foi criada fora da pasta publicada, em `../backups/marcello-site-antes-revisao-20261005-143919/`.

Os arquivos de autoria e verificação ficam em `../verificacao/site-revisado/`, fora da pasta publicada:

- `gerar_resumo.py`: gera PDF e HTML do resumo a partir dos textos da página principal.
- `verificar_site.py`: confere estrutura, caminhos, contatos, fatos do PDF, imagens e contrastes.
- `verificacao.json`: resultado das verificações automatizadas.
- `RELATORIO.md`: síntese da verificação e limitações.

Essas ferramentas usam o runtime de autoria do Codex (Python, ReportLab, Pillow, pypdf e Poppler). Não são dependências do site nem precisam ser enviadas à hospedagem. Ao modificar o conteúdo posteriormente, atualize o HTML principal e regenere os resumos para manter a consistência.

## GitHub Pages

Destino de publicação: repositório `consutecbr-wq/marcello`, branch `main`, com a página principal na raiz. O histórico Git preserva a versão anterior para recuperação.

Todos os recursos de interface usam caminhos relativos. Para atualizar a publicação, envie o conteúdo completo de `marcello-site/` ao destino já configurado para o site, mantendo `assets/`, os dois HTMLs e `.nojekyll`. Não envie as pastas de backup ou verificação. Verifique a pasta e branch usadas pela hospedagem antes de substituir arquivos.

A revisão não tem dependência de build. Após o envio e a conclusão do GitHub Pages, confira a versão servida em `https://consutecbr-wq.github.io/marcello/`, os contatos, o resumo em HTML e o PDF.
