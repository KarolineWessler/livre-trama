# Livre Trama — Memórias Bordadas à Mão

Uma Landing Page responsiva, fluida e feita com muito carinho, desenvolvida para o ateliê de bordado manual **Livre Trama**. O projeto foi estruturado com foco em um design minimalista, buscando trazer muito da estética já aplicada nos bordados e nas redes, alta performance, acessibilidade e semântica rigorosa.

---

## Design do Projeto

O planejamento visual, paleta de cores e tipografia foram desenhados e centralizados no Figma.

- **Link do Projeto no Figma:** [Design do Sistema - Livre Trama](https://www.figma.com/design/x5lXn4jmwVsplbiO6KkygG/Projetos?node-id=0-1&t=SW9Y2JRY2nTxCRaB-1)

---

## Como os Requisitos Foram Resolvidos

### 1. Estrutura Semântica Rigorosa

A página foi construída eliminando o uso excessivo de `<div>` genéricas. Foram utilizadas tags estruturais como `<header>`, `<main>`, `<section>`, `<article>` e `<footer>`, garantindo que a hierarquia do conteúdo seja perfeitamente interpretável por motores de busca (SEO) e leitores de tela.

### 2. Sistema de Design com Variáveis CSS

Centralização da identidade visual no bloco `:root` utilizando variáveis customizadas para cores (como `--bg-cream`, `--color-primary` e `--color-secondary`) e fontes (`--header-font`, `--body-font`). Isso permite que qualquer alteração estética na marca seja replicada globalmente de forma instantânea e organizada.

### 3. Layout Híbrido (Flexbox & CSS Grid)

Combinação estratégica das duas caixas de layout do CSS:

- **Flexbox:** Utilizado nos componentes de fluxo linear, como o alinhamento de itens do menu de navegação (`.nav-list`), centralização de blocos e botões de contato.
- **CSS Grid:** Aplicado na estruturação de grades complexas, como o mosaico de fotos do portfólio (`.portfolio-grid`) e a distribuição equilibrada de cards informativos.

### 4. Interface Responsiva

Implementação de design responsivo utilizando propriedades elásticas como `clamp()` para textos e larguras, além de Media Queries focadas em breakpoints estratégicos. A interface se adapta perfeitamente desde dispositivos móveis pequenos até monitores Desktop de alta resolução.

### 5. Microinterações de Feedback

Desenvolvimento de transições suaves (`transition`) em estados de `:hover` para links e botões. O mosaico de portfólio conta com efeitos sutis de escala (`scale`) nas imagens e elevação nos cards, enriquecendo a experiência sensorial do usuário ao navegar pelas obras.

### 6. Curadoria de Código com IA

Utilização de Inteligência Artificial para auxiliar na lógica e na estrutura de cards dinâmicos e responsivos. O código gerado passou por uma curadoria minuciosa para se adequar estritamente aos padrões de estilização (`BEM CSS`) e variáveis já estabelecidos no ecossistema do projeto.

### 7. Implementação de Dark Mode Nativo (Pesquisa)

Pesquisa e aplicação da Media Query prefers-color-scheme. Visando respeitar a estética afetiva, suave e artesanal do ateliê (composta por tons de linho, algodão cru e linhas terrosas), a estrutura da media query foi analisada, porém optei por não implementar a inversão tradicional de cores para o tema escuro, pois descaracterizaria a identidade visual e o conceito orgânico da marca, mantendo a paleta clara e confortável como padrão global do sistema.

### 8. Sticky Headers e Scroll Snap (Pesquisa)

- **Sticky Header:** O cabeçalho foi fixado no topo da tela utilizando `position: fixed` com um efeito moderno de desfoque de fundo através de `backdrop-filter: blur(10px)`.
- **Scroll Snap:** Aplicação de `scroll-snap-type: y proximity` no elemento `<html>` combinado com `scroll-snap-align: start` nas seções principais, criando transições de rolagem magnéticas e confortáveis para o usuário.

### 9. Otimização de Performance e Assets (Pesquisa)

Para garantir um carregamento instantâneo e buscar uma pontuação próxima a 100 no Google PageSpeed, foram aplicadas estratégias de otimização na renderização e no peso dos arquivos:

- **Conversão de Assets:** Todas as imagens de alta resolução foram convertidas para o formato moderno **WebP** através da ferramenta _AnyWebP_, reduzindo drasticamente o tamanho dos arquivos sem perder a nitidez dos pontos do bordado.
- **Preconnect de Fontes Externas:** Implementação de tags `<link rel="preconnect">` para o Google Fonts. Isso avisa o navegador para estabelecer uma conexão antecipada com o servidor de fontes, eliminando o atraso de DNS e agilizando o carregamento da tipografia.
- **Otimização de Carregamento de Fontes:** Uso do parâmetro `&display=swap` na URL das fontes, permitindo que o texto seja renderizado imediatamente com uma fonte nativa do sistema enquanto os arquivos customizados são baixados, evitando o efeito de "texto invisível" (_FOIT_).
- **SEO e Carregamento:** Inclusão de `<meta name="viewport">` configurada corretamente para evitar atrasos de clique em dispositivos móveis e uma `meta description` otimizada para indexação eficiente.

### 10. Acessibilidade Avançada com Teclado (Pesquisa)

Garantia de navegação completa sem o uso de mouse:

- Implementação do seletor `:focus-visible` com linhas pontilhadas customizadas (`outline-offset`), destacando claramente onde o foco do teclado está.
- Inclusão de classes utilitárias de acessibilidade (como `.sr-only`) para elementos textuais destinados exclusivamente a leitores de tela.

---

Achei muito divertido montar o site. Veio em uma hora perfeita, minha irmã precisava de uma landing page pro atelier de bordados e eu de um projeto. Decidimos a identidade visual juntas de acordo com as cores e elementos que ela já utiliza nos bordados e nas fotos de divulgação do instagram, fiz o design do que queria pra algumas páginas no figma e depois validei tudo com ela. Foi um processo gradual, tranquilo e feliz, unindo o desenvolvimento com arte. 🧵✨
