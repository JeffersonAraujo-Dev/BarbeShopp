# BarbeShopp — Modelo de site profissional para barbearias

**Demonstração online:** [Acesse o site BarbeShopp](https://barbeshopp.jefferson-dlufan.workers.dev/)

**Uma apresentação digital para valorizar a identidade da barbearia, divulgar seus serviços e facilitar o contato pelo WhatsApp.**

Projeto demonstrativo de uma landing page responsiva, desenvolvido com **HTML, CSS e JavaScript**. A proposta combina uma identidade visual contemporânea, informações objetivas e caminhos diretos para iniciar uma conversa sobre agendamento.

> **Projeto de portfólio:** BarbeShopp é um nome utilizado nesta demonstração. Este site é um modelo para barbearias e não representa um estabelecimento real atendido. Textos, serviços, valores e fotografias têm finalidade ilustrativa e devem ser personalizados antes de uma entrega comercial.

**Tem uma barbearia e quer uma apresentação como esta para o seu negócio?** A estrutura pode ser adaptada à sua marca, aos seus serviços e à forma como você atende seus clientes. Para conhecer outros projetos e conversar sobre uma proposta, acesse o [perfil do desenvolvedor no GitHub](https://github.com/JeffersonAraujo-Dev).

## Sumário

- [Apresentação e objetivo](#apresentação-e-objetivo)
- [Experiência do visitante](#experiência-do-visitante)
- [Funcionalidades implementadas](#funcionalidades-implementadas)
- [Tecnologias e organização](#tecnologias-e-organização)
- [Como executar o projeto](#como-executar-o-projeto)
- [Como personalizar para uma barbearia](#como-personalizar-para-uma-barbearia)
- [Funcionamento do WhatsApp](#funcionamento-do-whatsapp)
- [Responsividade e acessibilidade](#responsividade-e-acessibilidade)
- [Publicação e atualização](#publicação-e-atualização)
- [Processo de adaptação e entrega](#processo-de-adaptação-e-entrega)
- [Verificação antes da divulgação](#verificação-antes-da-divulgação)
- [Solução de problemas](#solução-de-problemas)
- [Escopo e possíveis evoluções](#escopo-e-possíveis-evoluções)
- [Créditos e apresentação profissional](#créditos-e-apresentação-profissional)

## Apresentação e objetivo

O BarbeShopp demonstra como uma barbearia pode apresentar sua identidade e seus serviços em uma página própria. A organização foi pensada para que o visitante entenda a proposta do estabelecimento, consulte os serviços e encontre uma forma de contato sem precisar navegar por diversas telas.

O projeto também funciona como uma amostra de serviços de desenvolvimento web: criação de páginas institucionais, organização de conteúdo, implementação de layouts responsivos e integração de links de atendimento.

### O que pode ser personalizado

| Elemento | Possibilidade de adaptação |
| --- | --- |
| Marca | Nome, logotipo e assinatura visual da barbearia |
| Identidade | Cores, tipografia, fotografias e linguagem dos textos |
| Serviços | Nomes, descrições, quantidade de opções e preços |
| Atendimento | Número do WhatsApp e mensagens de primeiro contato |
| Conteúdo institucional | História, proposta e diferenciais verificáveis do estabelecimento |
| Publicação | Nome do projeto e endereço de acesso escolhido na hospedagem |

O resultado é uma base de apresentação comercial. A personalização deve refletir a operação real de cada cliente; nenhum resultado de vendas ou volume de agendamentos é garantido pelo modelo.

## Experiência do visitante

1. **Primeiro contato com a marca:** a abertura apresenta uma fotografia, o nome da barbearia, uma mensagem principal e o convite para reservar um horário.
2. **Consulta aos serviços:** os cartões mostram corte masculino, barba completa e combo, acompanhados de descrições e preços iniciais.
3. **Conhecimento da proposta:** a seção institucional apresenta o ambiente e a abordagem de atendimento por meio de texto e imagem.
4. **Início do atendimento:** a área de contato e o botão flutuante direcionam ao WhatsApp quando o número está configurado.
5. **Combinação do horário:** o visitante envia a mensagem e a equipe verifica a disponibilidade durante a conversa.

**O clique no botão não confirma uma reserva.** O site prepara o contato; a confirmação do serviço, do preço e do horário acontece com a barbearia.

## Funcionalidades implementadas

| Recurso | Comportamento atual |
| --- | --- |
| Página única | Abertura, serviços, apresentação institucional, contato e rodapé |
| Navegação interna | Links levam às seções por identificadores como `#servicos` e `#contato` |
| Menu para celular | Botão de abertura e fechamento em telas menores, quando o JavaScript está ativo |
| Cartões de serviços | Nome, descrição, preço inicial e chamada para agendamento |
| WhatsApp flutuante | Botão circular no canto inferior direito, disponível durante a navegação |
| Mensagem por serviço | O link do cartão informa o serviço escolhido na mensagem preparada |
| Configuração centralizada | Um único número no JavaScript alimenta os links de atendimento |
| Aviso de configuração | Os botões gerais avisam quando não há número válido informado |
| Ano do rodapé | Atualizado pelo JavaScript a partir da data do dispositivo |
| Fotografias locais | Imagens incluídas em `assets/`, sem depender do Unsplash para carregar a página |
| Metadados básicos | Idioma, título, descrição, viewport e cor de tema definidos no HTML |

Os botões da abertura e do menu levam primeiro à seção de contato. Os botões identificados para WhatsApp e os links dos cartões recebem o endereço externo quando a configuração é válida.

## Tecnologias e organização

| Tecnologia | Responsabilidade |
| --- | --- |
| HTML | Estrutura, conteúdo, links, imagens e significado dos elementos |
| CSS | Cores, tipografia, espaçamento, posicionamento, estados visuais e adaptação de tela |
| JavaScript | Menu, mensagens de WhatsApp, aviso temporário e atualização do ano |

O projeto é estático e utiliza recursos nativos do navegador. Não exige instalação de pacotes, compilação, framework, servidor de aplicação ou banco de dados para a experiência atual.

### Estrutura da pasta distribuída

| Caminho | Conteúdo |
| --- | --- |
| `index.html` | Página principal |
| `css/style.css` | Folha de estilos, organizada por seções |
| `js/script.js` | Comportamentos e configuração do WhatsApp |
| `assets/hero.jpg` | Fotografia da abertura |
| `assets/barba.jpg` | Fotografia da seção institucional |
| `LEIA-ME.txt` | Orientações rápidas incluídas no pacote |
| `README.md` | Esta documentação; coloque-a na raiz do repositório |

Os caminhos acima consideram a pasta **BarbeShopp** após extrair o ZIP. Caso o repositório mantenha os arquivos públicos dentro de `dist/`, esses mesmos caminhos ficam sob `dist/`; a pasta de publicação deve acompanhar essa organização.

### Organização do CSS

O arquivo reúne blocos para paleta e base, navegação, abertura, serviços, apresentação e contato, botão de WhatsApp e adaptações de tela. As variáveis em `:root` concentram as principais cores para simplificar a personalização.

## Como executar o projeto

### Abertura direta

1. Baixe e extraia o pacote do projeto.
2. Abra a pasta que contém `index.html`.
3. Mantenha as pastas `css`, `js` e `assets` junto desse arquivo.
4. Abra `index.html` em um navegador.

A apresentação pode ser visualizada localmente. O acesso ao WhatsApp precisa de conexão com a internet.

### Edição no VS Code

1. Abra o VS Code e selecione **Arquivo → Abrir Pasta**.
2. Escolha a pasta do projeto completo.
3. Edite o conteúdo no HTML, o visual no CSS e o atendimento no JavaScript.
4. Salve as alterações e atualize a página no navegador.

### Servidor local opcional

Se o Python 3 estiver instalado, abra um terminal na pasta que contém `index.html` e execute:

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Abra `http://127.0.0.1:8000` no navegador. Para encerrar, pressione `Ctrl + C` no terminal. Essa alternativa serve para visualização no próprio computador; ela não publica o site na internet.

## Como personalizar para uma barbearia

### 1. Identificação e textos

No `index.html`, substitua o nome BarbeShopp no título da página, na marca, nos textos, nas descrições acessíveis e no rodapé. Atualize também as referências à marca no JavaScript, incluindo as mensagens de atendimento.

Revise a descrição usada pelos mecanismos de busca:

```html
<title>Nome da Barbearia | Corte e barba</title>
<meta
  name="description"
  content="Conheça os serviços da Nome da Barbearia em sua cidade e entre em contato para agendar."
>
```

O título e a descrição devem apresentar informações reais e específicas. A existência dessas tags não garante posição nos resultados de pesquisa.

### 2. Cores e identidade

As cores principais estão em `css/style.css`:

```css
:root {
  --dark: #151715;
  --dark-soft: #20231f;
  --gold: #d3b077;
  --paper: #f3f1e9;
  --muted: #b9bcb4;
  --ink: #222720;
}
```

Altere essas variáveis conforme a identidade da barbearia. Depois da alteração, confira a leitura de textos e botões sobre fundos claros e escuros. Há também cores específicas em outros seletores; uma revisão completa da identidade deve considerar esses valores.

### 3. Serviços e preços

Cada serviço está em um elemento `article` com a classe `card`. Para editar uma opção, atualize o título, a descrição, o preço, o atributo `data-service` e o texto de `aria-label` do link.

```html
<a
  href="#contato"
  class="service-link"
  data-service="Corte masculino"
  aria-label="Agendar corte masculino"
>↗</a>
```

O atributo `data-service` informa ao JavaScript qual nome inserir na mensagem de WhatsApp. Alterar apenas o título visível do cartão não altera automaticamente esse atributo.

Os valores do modelo são **R$ 45 para corte**, **R$ 35 para barba** e **R$ 70 para combo**, apresentados como preços iniciais. Eles devem ser confirmados ou substituídos pelo estabelecimento.

### 4. Fotografias

Substitua as imagens de `assets/` por fotografias autorizadas da barbearia, da equipe, dos instrumentos ou dos trabalhos realizados. Você pode manter os nomes existentes ou atualizar os caminhos `src` no HTML.

Ao trocar uma fotografia:

1. Ajuste o atributo `alt` para descrever o novo conteúdo.
2. Revise as dimensões declaradas e o enquadramento.
3. Confira o corte da imagem no computador e no celular.
4. Comprima o arquivo para evitar downloads desnecessariamente grandes.

O CSS usa `object-fit: cover`; isso preenche o espaço disponível, mas pode recortar partes da foto. O atributo visual `object-position` permite ajustar qual região recebe destaque.

### 5. Informações locais

Endereço, horário de funcionamento, redes sociais e mapa não estão implementados nesta versão. Esses dados podem ser acrescentados como parte da adaptação para um cliente, depois de confirmados com a barbearia.

## Funcionamento do WhatsApp

### Número de atendimento

Abra `js/script.js` e localize:

```js
const WHATSAPP_NUMBER = "";
const DEFAULT_MESSAGE = "Olá! Gostaria de agendar um horário na BarbeShopp.";
```

Preencha a primeira constante com o número real no formato **55 + DDD + número**, entre aspas e somente com dígitos. Não inclua `+`, espaços, hífens ou parênteses.

A verificação atual aceita sequências brasileiras com **12 ou 13 dígitos**, iniciadas por `55`. Essa checagem verifica o formato; ela não confirma que a conta existe no WhatsApp.

### Como os links são montados

O JavaScript percorre os elementos com `data-whatsapp` ou `data-service`. Com um número válido, monta um link `wa.me`, inclui a mensagem com `encodeURIComponent` e configura a abertura em nova aba.

| Origem do contato | Mensagem preparada |
| --- | --- |
| Botão flutuante ou botão da seção de contato | Texto definido em `DEFAULT_MESSAGE` |
| Link de um cartão | Saudação acompanhada do nome informado em `data-service` |

O usuário ainda precisa enviar a mensagem no WhatsApp. O site não envia mensagens automaticamente nem consulta a agenda da equipe.

### Quando o número está vazio ou fora do formato

- Os botões gerais do WhatsApp exibem um aviso temporário.
- Os links dos serviços continuam levando à seção de contato.
- Nenhuma conversa é aberta com um número fictício.

Para apresentar o modelo no portfólio, é possível manter o atendimento sem configuração. Se utilizar seu próprio número para receber interessados no desenvolvimento, altere as mensagens e sinalize claramente que o contato é para solicitar um site, não para marcar um corte.

## Responsividade e acessibilidade

O layout utiliza Flexbox, CSS Grid, tamanhos fluidos e regras por largura de tela. Em telas maiores, os serviços aparecem em três colunas e a seção institucional divide imagem e texto. Em telas menores, o conteúdo passa para uma coluna e a navegação usa um botão de menu.

Entre os recursos implementados estão:

- Idioma da página definido como português do Brasil.
- Elementos semânticos como `header`, `nav`, `main`, `section` e `footer`.
- Link para pular diretamente ao conteúdo principal.
- Indicadores visíveis de foco para links e botões.
- Rótulos acessíveis em controles representados por ícones.
- Estado de expansão do menu informado por `aria-expanded`.
- Fechamento do menu com `Escape` e devolução do foco ao botão.
- Preferência por movimento reduzido respeitada no CSS.
- Aviso de configuração com `role="status"`.

Sem JavaScript, o conteúdo continua visível e a navegação permanece expandida; a montagem dos links de WhatsApp e os demais comportamentos dinâmicos dependem do script.

Esses recursos não equivalem a uma certificação de acessibilidade. Uma entrega comercial deve incluir verificação com teclado, ampliação de texto, dispositivos reais e, conforme o escopo, tecnologias assistivas.

## Publicação e atualização

### Publicar sem comprar um domínio

O Cloudflare Pages permite publicar arquivos estáticos e fornece um endereço no formato `nome-do-projeto.pages.dev`. O nome efetivo depende da disponibilidade. Veja a [documentação de envio direto](https://developers.cloudflare.com/pages/get-started/direct-upload/).

1. Crie ou acesse sua conta na Cloudflare.
2. Entre em **Workers & Pages** e escolha a criação de uma aplicação Pages por envio de arquivos.
3. Extraia o pacote e selecione a pasta que contém diretamente `index.html`, `css/`, `js/` e `assets/`.
4. Informe um nome para o projeto e envie os arquivos.
5. Publique e aguarde a confirmação.
6. Abra o endereço retornado e confira a página e os links.

Não envie uma pasta externa que deixe o `index.html` escondido em mais um nível. Para atualizar, crie uma nova publicação no mesmo projeto com a pasta revisada.

Projetos criados por envio direto não podem ser convertidos posteriormente para integração Git no mesmo projeto; essa mudança exige outro projeto Pages. Os nomes das opções do painel podem mudar. [Referência oficial](https://developers.cloudflare.com/pages/get-started/direct-upload/).

### Organização para publicação a partir de um repositório

O site não possui etapa de compilação. O diretório público deve ser aquele que contém o `index.html`: a raiz da pasta extraída ou `dist/`, se essa organização for mantida no repositório. Consulte o [guia oficial de HTML estático](https://developers.cloudflare.com/pages/framework-guides/deploy-anything/) para a configuração vigente da plataforma.

Mantenha este README na raiz do repositório para que sirva como apresentação do projeto. A demonstração pode ser acessada em [BarbeShopp — site demonstrativo](https://barbeshopp.jefferson-dlufan.workers.dev/). O endereço divulgado utiliza o subdomínio `workers.dev`; as instruções de Cloudflare Pages acima são uma alternativa de publicação.

## Processo de adaptação e entrega

O fluxo abaixo descreve como este modelo pode orientar a execução de um serviço para uma barbearia. Prazo, preço, revisões e manutenção devem ser combinados para cada projeto.

| Etapa | Atividade | Resultado esperado |
| --- | --- | --- |
| 1. Levantamento | Entender o negócio, público, identidade, serviços e forma de atendimento | Lista de conteúdo e necessidades confirmadas |
| 2. Definição do escopo | Combinar quais seções, integrações e adaptações serão entregues | Proposta com entregáveis e limites claros |
| 3. Coleta de materiais | Receber marca, fotos, textos, preços e contato autorizados | Conteúdo disponível para personalização |
| 4. Implementação | Adaptar HTML, CSS e JavaScript à identidade aprovada | Versão navegável do site |
| 5. Revisão | Conferir conteúdo, leitura, navegação e atendimento | Ajustes e aprovação da versão final |
| 6. Publicação | Enviar os arquivos para a hospedagem escolhida | Endereço acessível para divulgação |
| 7. Entrega | Disponibilizar arquivos, acessos acordados e orientações | Cliente apto a utilizar e divulgar o site |
| 8. Manutenção | Atualizar informações conforme contratação | Conteúdo acompanhado ao longo do uso |

## Verificação antes da divulgação

Esta lista é um roteiro de conferência, não uma declaração de testes já concluídos.

- [ ] Marca, textos e fotografias correspondem ao estabelecimento ou estão identificados como demonstração.
- [ ] Valores e descrições foram revisados.
- [ ] Número de WhatsApp e mensagens estão corretos.
- [ ] Botão flutuante, contato e links dos três serviços foram conferidos.
- [ ] Menu abre, fecha e responde ao teclado.
- [ ] Página foi examinada em larguras como 320, 375, 768, 1024 e 1440 pixels.
- [ ] Não há rolagem horizontal involuntária nem conteúdo sobreposto.
- [ ] Textos permanecem utilizáveis com ampliação de 200%.
- [ ] Fotografias e arquivos carregam no endereço publicado.
- [ ] Título e descrição da página foram personalizados.
- [ ] Console do navegador não apresenta erros de JavaScript.
- [ ] Link público confirmado foi incluído no portfólio e nos canais de divulgação.

## Solução de problemas

| Sintoma | O que verificar |
| --- | --- |
| A página aparece sem estilo | Caminho `css/style.css`, nome da pasta e envio do arquivo |
| As imagens não carregam | Caminhos em `src`, extensão dos arquivos e diferença entre maiúsculas e minúsculas |
| O menu mobile não responde | Carregamento de `js/script.js` e erros no console |
| O WhatsApp mostra um aviso | Preenchimento de `WHATSAPP_NUMBER` conforme o formato exigido |
| O WhatsApp abre o destinatário errado | Número completo, DDD e código do país |
| O nome do serviço na mensagem está errado | Valor de `data-service` no cartão correspondente |
| O site publicado retorna página não encontrada | Existência de `index.html` na raiz do diretório enviado |
| As alterações não aparecem | Arquivos salvos, nova publicação concluída e cache do navegador |

## Escopo e possíveis evoluções

### Incluído nesta versão

Site institucional estático, apresentação de serviços, layout responsivo, menu mobile, fotografias locais e contato pelo WhatsApp.

### Não implementado

Agenda automática, seleção de horários em tempo real, painel administrativo, cadastro de clientes, autenticação, pagamentos, envio de e-mails, formulário de contato, métricas de conversão e integrações com sistemas de gestão.

### Possibilidades para um projeto futuro

Galeria de trabalhos, perfis dos profissionais, endereço e mapa, depoimentos autorizados, compartilhamento social aprimorado ou conexão com uma plataforma de agendamento. Esses recursos exigem definição de escopo e implementação adicional; não fazem parte da entrega atual.

## Créditos e apresentação profissional

**Apresentação de portfólio:** Ifákáyọ̀dé — [JeffersonAraujo-Dev no GitHub](https://github.com/JeffersonAraujo-Dev).

O projeto demonstra competências em estruturação de páginas, estilização responsiva, JavaScript no navegador e preparação de arquivos para hospedagem estática.

### Fotografias

As imagens ilustrativas foram obtidas do Unsplash e incluídas localmente:

- [Imagem da abertura](https://images.unsplash.com/photo-1503951914875-452162b0f3f1)
- [Imagem da seção institucional](https://images.unsplash.com/photo-1621605815971-fbc98d665033)

Consulte os [termos de uso das imagens do Unsplash](https://unsplash.com/license). Em uma personalização comercial, fotografias autorizadas do próprio estabelecimento ajudam a apresentar o ambiente e os trabalhos reais.

### Interesse em um projeto personalizado

**Sua barbearia pode ter uma página com a sua identidade, seus serviços e seu canal de atendimento.** Este modelo é um ponto de partida para discutir uma solução adequada ao negócio.

Conheça o [perfil do desenvolvedor](https://github.com/JeffersonAraujo-Dev) para acompanhar outros projetos e consultar os canais de contato disponibilizados. O escopo final, a publicação, as revisões e a manutenção são definidos na proposta de cada serviço.
