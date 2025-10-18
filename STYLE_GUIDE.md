🎨 ORBENT STYLE GUIDE
Versão: 1.0 • Data: 18/10/2025
Documento: Guia de Identidade Visual e Diretrizes Técnicas do Sistema de Marca Orbent

---

1. CONCEITO DE MARCA

A Orbent é uma marca que simboliza tecnologia, inteligência e cultura organizacional.
Sua estética combina **precisão técnica** e **inspiração humana**, refletindo clareza, modernidade e propósito.

Slogan oficial:
“Visão sistêmica. Cultura viva. Inteligência com propósito.”

---

2. ESTRUTURA DA IDENTIDADE

Logo corporativa → versão principal, aplicada em fundos azul Orbent.
Logo clara → utilizada em fundos escuros (dark mode).
Logo escura → utilizada em fundos claros.
Logo com slogan → utilizada em materiais institucionais e apresentações.
Ícone Orbent → aplicação reduzida (favicons, aplicativos e barras laterais).

---

3. PALETA DE CORES

Azul Orbent: #001434 – cor base e fundo institucional
Azul Acento: #5271FF – interações, destaques e links
Dourado Orbent: #CCA300 – elementos de ênfase e detalhes premium
Branco Gelo: #FDFDFD – fundo claro e contraste
Cinza Neutro: #6B7280 – texto auxiliar e elementos secundários

Arquivo de referência: assets/palette.png

---

4. TIPOGRAFIA OFICIAL

Primária: Inter (pesos 400–700) → corpo de texto e conteúdos técnicos
Secundária (Display): Poppins (pesos 600–800) → títulos, slogans e cabeçalhos
Fallback universal: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial

As fontes devem ser importadas via Google Fonts em todos os produtos Orbent.

---

5. GRID E ESPAÇAMENTO

Unidade base: 4 px
Escala de espaçamento: 4 / 8 / 12 / 16 / 20 / 24 / 32 / 48 px

Tokens correspondentes no CSS:
--size-1 = 4px
--size-4 = 16px
--size-7 = 32px
--radius-md = 8px

Layout recomendado:

* Containers com largura máxima de 1120 px
* Margens internas amplas e proporcionais
* Evitar sobreposição visual ou excesso de densidade

---

6. LOGOTIPO

Zona de proteção:
A área mínima livre ao redor da marca deve ser igual à altura do “O” do logotipo.

Tamanhos mínimos:
• Impressão: 30 mm
• Web: 160 px
• Ícone ou favicon: 32 px

Fundos recomendados:
• Azul Orbent (#001434)
• Branco Gelo (#FDFDFD)
• Cinza neutro claro (#F5F7FA)

Evitar: fundos coloridos vibrantes, gradientes conflitantes ou imagens ruidosas.

Variações de uso:
• logo-corporativa.png → principal
• orbent-logo-claro.png → fundo escuro
• orbent-logo-escuro.png → fundo claro
• logo-slogan.png → comunicações institucionais

---

7. ELEMENTOS GRÁFICOS E PATTERNS

Os padrões visuais da Orbent representam **energia, conectividade e fluxo de dados**.

Pattern base: pattern.png → fundo neutro e genérico
Pattern translúcido: pattern_opacidade.png → sobreposições sutis e cabeçalhos
Pattern galáxia: Pattern-galaxia.png → hero sections e telas de destaque
Hero oficial: Hero Section.jpeg → aplicação em apresentações e banners

Exemplo de aplicação CSS:
.bg-orbent {
background-color: #001434;
background-image: url('../assets/pattern/pattern_opacidade.png');
background-size: cover;
}

---

8. GRADIENTE DE IDENTIDADE

Gradiente oficial: linear-gradient(45deg, #f8ad00 0%, #e13333 50%, #3992ff 100%)

Representa os três pilares da Orbent:
• Energia → inovação contínua
• Transformação → integração tecnológica
• Inteligência → clareza e decisão

Usos recomendados:

* Títulos com classe .gradient-orbent
* Botões de ação
* Barras de progresso e indicadores
* Ícones e detalhes de destaque

---

9. WHITE LABEL E SUBMARCAS

O sistema Orbent é totalmente white-label, permitindo personalização controlada pelos clientes.
A estrutura visual deve manter o selo “by Orbent” em todas as derivações.

Exemplo: <span class="brand-ribbon">
ACME <span class="brand-ribbon__by">by Orbent</span> </span>

Regra: o selo “by Orbent” nunca deve ser removido nem reduzido abaixo de 60% da largura da marca principal.

---

10. DIRETRIZES DE CONSISTÊNCIA

11. Usar apenas cores e fontes oficiais.

12. Preservar proporções e legibilidade do logotipo.

13. Utilizar apenas arquivos originais (SVG ou PNG).

14. Manter margens e áreas de respiro.

15. Aplicar em fundo sólido e com contraste adequado.

16. Evitar distorções, sombras extras e efeitos não previstos.

---

11. GUIA TÉCNICO (CSS GUIDE)

O CSS Guide complementa este documento e está localizado em /css/orbent.css.
Contém tokens, variáveis, temas, utilitários e componentes do design system.

---

12. CRÉDITOS E LICENÇA

© Orbent — Todos os direitos reservados.
Distribuição autorizada apenas para uso interno e clientes licenciados by Orbent.
Reprodução parcial, alteração ou redistribuição é proibida sem autorização formal.

---

13. ATUALIZAÇÃO

Este guia será revisado a cada nova versão do produto.
Próxima atualização prevista: Q1/2026.

---

🧩 ORBENT CSS GUIDE
Versão: 1.0 • Data: 18/10/2025
Documento: Guia técnico do Design System Orbent
Arquivo base: /css/orbent.css

---

1. OBJETIVO

O CSS Guide descreve o uso técnico do arquivo orbent.css — incluindo tokens, temas, tipografia, layouts e componentes reutilizáveis.
Sua função é garantir consistência visual, acessibilidade e escalabilidade em todos os produtos da Orbent e clientes white-label.

---

2. ESTRUTURA

orbent.css contém:

* Reset e normalização
* Tokens globais (:root)
* Temas (light/dark)
* Tipografia
* Layouts e utilitários
* Componentes base
* Patterns e gradientes
* White-label overrides

---

3. TOKENS

:root {
--orb-primary: #001434;
--orb-accent: #5271FF;
--orb-gold: #CCA300;
--orb-white: #FDFDFD;
--orb-gradient: linear-gradient(45deg, #f8ad00, #e13333, #3992ff);
--font-sans: "Inter", system-ui, sans-serif;
--font-display: "Poppins", var(--font-sans);
--radius-md: 8px;
--shadow-md: 0 8px 24px rgba(0, 0, 0, 0.08);
}

---

4. TEMAS

<body class="theme-light"> … </body>  
<body class="theme-dark"> … </body>  

Tokens principais:
--bg: #FDFDFD / #0E121A
--text: #1F2430 / #E6E9F0
--surface: #F5F7FA / #121826
--brand: #001434 / #2A64FF

---

5. TIPOGRAFIA

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Poppins:wght@600;700&display=swap" rel="stylesheet">  

Elementos:
h1 → Poppins 2.5rem 700
h2 → Poppins 2rem 600
p → Inter 1rem 400
.subtitle → Inter 1rem 500
.caption → Inter 0.875rem 400

---

6. COMPONENTES

Botões: <button class="btn">Primário</button> <button class="btn btn--outline">Outline</button> <button class="btn btn--gradient">Gradient</button> <button class="btn btn--gold">Dourado</button>

Cards:

<div class="card">
  <div class="card__header"><h3>Título</h3></div>
  <div class="card__body">Conteúdo...</div>
</div>  

Badges: <span class="badge badge--gradient">Ativo</span> <span class="badge badge--gold">Premium</span>

Alertas:

<div class="alert alert--info">Informação</div>  
<div class="alert alert--success">Sucesso!</div>  
<div class="alert alert--warning">Atenção</div>  
<div class="alert alert--danger">Erro!</div>  

Tabelas:

<table class="table table--compact">
  <thead><tr><th>Coluna</th></tr></thead>
  <tbody><tr><td>Dado</td></tr></tbody>
</table>  

---

7. LAYOUTS E GRID

.container → largura máxima de 1120px
.grid → display grid com espaçamento padrão
.cols-2 / .cols-3 → controle de colunas
.section → padding vertical padrão

---

8. PATTERNS E FUNDOS

.bg-orbent {
background-color: #001434;
background-image: url('../assets/pattern/pattern_opacidade.png');
}

.bg-orbent--galaxy {
background-image: url('../assets/pattern/Pattern-galaxia.png');
}

<section class="hero bg-orbent--galaxy">
  <h1 class="gradient-orbent">Orbent</h1>
</section>  

---

9. HERO SECTION

<section class="hero">
  <div class="container">
    <h1 class="gradient-orbent">Orbent</h1>
    <p class="subtitle">Visão sistêmica. Cultura viva.<br>Inteligência com propósito.</p>
  </div>
</section>  

.hero → espaçamento institucional
.gradient-orbent → gradiente oficial aplicado ao texto

---

10. WHITE LABEL

:root.brand-client {
--orb-primary: #0E3A5B;
--orb-accent: #00C48C;
--orb-gold: #FF7A59;
}

<span class="brand-ribbon">
  ACME <span class="brand-ribbon__by">by Orbent</span>
</span>  

---

11. BOAS PRÁTICAS

12. Use variáveis (--orb-*) para cores e dimensões.

13. Não sobrescreva estilos base — crie extensões (.btn--cliente).

14. Mantenha contraste mínimo 4.5:1.

15. Prefira sombras e gradientes sutis.

16. Siga os tokens oficiais e padrões de espaçamento.

---

12. HISTÓRICO DE VERSÕES

v1.0 – 18/10/2025
• Criação do CSS Guide e integração com orbent.css

v1.1 – Q1/2026
• Inclusão de toolbar, tabela responsiva e form-kit

---

© Orbent Design System — Todos os direitos reservados.
Distribuição autorizada apenas para produtos e clientes by Orbent.
