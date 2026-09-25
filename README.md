# Projeto: Geometria Interativa com CSS Puro

Este projeto é uma aplicação web desenvolvida para demonstrar o uso de **CSS3 moderno** (Grid Layout, Flexbox e `clip-path`) na criação e estilização de **10 formas geométricas planas** e na exibição de suas respectivas fórmulas matemáticas de área e perímetro.

---

## 📋 Requisitos do Projeto

1. **Estrutura de Arquivos Separados**: Arquivos `index.html` e `styles.css` vinculados de forma externa através da tag `<link rel="stylesheet" href="styles.css">`.
2. **Layout Responsivo com CSS Grid**: Organização dos cards de figuras em uma grade dinâmica e adaptável para diferentes tamanhos de tela.
3. **Alinhamentos e Distribuição com Flexbox**: Utilização de Flexbox para estruturação interna dos elementos do cabeçalho, hero section, cards e centralização do conteúdo dentro das formas geométricas.
4. **Formas Geométricas em CSS Puro**: Renderização visual de 10 figuras planas sem a necessidade de imagens externas ou SVGs, utilizando propriedades avançadas de CSS.

---

## 📐 Figuras Geométricas Implementadas

O projeto traz a representação visual e matemática das seguintes 10 formas:

1. **Quadrado**: Criado com dimensões iguais e `border-radius`.
2. **Círculo**: Estilizado com `border-radius: 50%`.
3. **Retângulo**: Proporções retangulares com bordas levemente arredondadas.
4. **Elipse**: Formato oval definido por `border-radius: 50%` com proporções de largura e altura distintas.
5. **Losango**: Estruturado via transformação espacial `transform: rotate(45deg)`.
6. **Triângulo**: Recortado com `clip-path: polygon(...)`.
7. **Trapézio**: Modelado através de polígono customizado em `clip-path`.
8. **Paralelogramo**: Aplicada a inclinação lateral com `transform: skewX(-20deg)`.
9. **Pentágono**: Definido por recorte de 5 vértices via `clip-path`.
10. **Hexágono**: Construído com polígono regular de 6 vértices via `clip-path`.

---

## 🛠️ Conceitos e Técnicas de CSS Utilizadas

### Layout e Estrutura
- **`display: grid` & `grid-template-columns: repeat(auto-fit, minmax(260px, 1fr))`**: Cria uma grade completamente responsiva que reajusta a quantidade de colunas automaticamente sem a necessidade de múltiplas media queries.
- **`display: flex`**: Empregado no cabeçalho, no container central das figuras e nas caixas de texto para alinhamento vertical e horizontal dos conteúdos (`justify-content` e `align-items`).
- **`gap`**: Definição de espaçamentos limpos e uniformes entre os elementos do grid.

### Estilização de Formas
- **`clip-path: polygon(...)`**: Recorte preciso de polígonos complexos diretamente no CSS.
- **`transform` (`rotate` e `skewX`)**: Manipulação de rotação e inclinação para criar os formatos de losango e paralelogramo.
- **`backdrop-filter: blur(...)`**: Efeito de desfoque de fundo no badge do cabeçalho.
- **`transition` & `:hover`**: Microinterações nos cards para feedback visual de elevação ao passar o mouse (`translateY`).

---

## 📱 Responsividade
O layout adapta-se automaticamente a telas mobile, tablets e desktops graças ao uso de unidades relativas e ao comportamento do `auto-fit` no CSS Grid.

---

## 📂 Como Executar o Projeto
1. Certifique-se de salvar os arquivos `index.html` e `styles.css` no mesmo diretório.
2. Abra o arquivo `index.html` em qualquer navegador web moderno.