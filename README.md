# Projeto: Flexbox e Formas Geométricas em CSS

Este projeto é uma aplicação prática desenvolvida para demonstrar o uso do **Box Model** do CSS e a manipulação de elementos usando o **Flexbox Layout**, aplicando conceitos de responsividade e estilização moderna através de formas geométricas recortadas e personalizadas.

---

## 📋 Requisitos da Atividade

1. **Estrutura de Arquivos Externa**: Criação dos arquivos `index.html` e `style.css`, conectando o CSS externamente via tag `<link rel="stylesheet">` no cabeçalho HTML.
2. **Manipulação do Box Model (20 Elementos)**:
   - Inclusão de 20 elementos distintos (`<div>`).
   - Atribuição explicita de valores para todas as quatro camadas do **Box Model**:
     - **Content** (`width`, `height`)
     - **Padding**
     - **Border**
     - **Margin**
3. **Aplicação do Flexbox (20 Propriedades)**: Utilização de 20 propriedades Flexbox distribuídas entre o *Flex Container* e os *Flex Items* para organizar a interface de maneira responsiva.

---

## 📐 Conceitos Aplicados

### 1. Box Model & Formas Geométricas
Cada um dos 20 elementos possui dimensões explicitamente definidas de largura/altura, espaçamentos internos (padding), bordas e margens externas. Para transformar os elementos retangulares tradicionais nas formas geométricas vistas em tela, foram utilizadas as seguintes técnicas de CSS:
- **`border-radius: 50%`**: Para a criação de círculos.
- **`clip-path: polygon(...)`**: Para recortar o elemento em formas como triângulos, losangos, pentágonos, hexágonos, octógonos, estrelas, cruzes e corações.

---

## 🛠️ Relação das 20 Propriedades de Flexbox Utilizadas

### No Flex Container (`.flex-container`)
1. **`display: flex;`** — Define o elemento pai como um container flexível.
2. **`flex-direction: row;`** — Organiza os itens em linha (direção horizontal principal).
3. **`flex-wrap: wrap;`** — Permite que os itens quebrem para a próxima linha caso não caibam na mesma.
4. **`justify-content: space-around;`** — Distribui os elementos uniformemente ao longo do eixo principal com espaço ao redor.
5. **`align-items: center;`** — Alinha os elementos no centro ao longo do eixo transversal (vertical).
6. **`align-content: space-between;`** — Distribui as linhas do container com espaço entre elas.
7. **`gap: 25px;`** — Define um espaçamento geral entre os itens flexíveis.
8. **`row-gap: 30px;`** — Define o espaçamento específico entre as linhas de itens.
9. **`column-gap: 20px;`** — Define o espaçamento específico entre as colunas de itens.

### Nos Flex Items (`.card-01` até `.card-11`)
10. **`order: 3;`** (`.card-01`) — Altera a ordem padrão de exibição do elemento na fila flex.
11. **`flex-grow: 1;`** (`.card-02`) — Define a taxa de crescimento do item em relação ao espaço sobressalente.
12. **`flex-shrink: 2;`** (`.card-03`) — Define a capacidade de encolhimento do item caso haja falta de espaço.
13. **`flex-basis: 120px;`** (`.card-04`) — Estabelece o tamanho inicial padrão do item antes da distribuição do espaço.
14. **`align-self: flex-start;`** (`.card-05`) — Sobrescreve o alinhamento vertical geral para alinhar este item ao topo.
15. **`align-self: flex-end;`** (`.card-06`) — Alinha este item individualmente na base da linha.
16. **`align-self: center;`** (`.card-07`) — Alinha este item individualmente no centro vertical da linha.
17. **`align-self: stretch;`** (`.card-08`) — Estica o item individual para ocupar toda a altura da linha.
18. **`flex: 1 1 110px;`** (`.card-09`) — Propriedade atalho (*shorthand*) combinando `flex-grow`, `flex-shrink` e `flex-basis`.
19. **`order: -1;`** (`.card-10`) — Move o item para o início absoluto do layout alterando sua prioridade visual.
20. **`align-self: baseline;`** (`.card-11`) — Alinha o item individualmente ao longo da linha base do texto do container.

---

## 📱 Responsividade
Uma media query `@media (max-width: 600px)` foi configurada para reorganizar a orientação do container de `row` para `column` em dispositivos móveis, garantindo visualização adequada.

---

## 📂 Como Executar o Projeto
1. Salve o arquivo `index.html` e o arquivo `style.css` na mesma pasta.
2. Abra o arquivo `index.html` em qualquer navegador web moderno.
