
```markdown
# 🌌 ORBENT BRAND ASSETS

Repositório oficial de **identidade visual**, **tokens de design** e **componentes CSS** da plataforma **Orbent** — um ecossistema white-label que une tecnologia, inteligência e cultura organizacional.

> “Visão sistêmica. Cultura viva. Inteligência com propósito.”

---

## 📦 Estrutura


orbent-brand-assets/
├── README.md
├── STYLE_GUIDE.md
├── CSS_GUIDE.md
├── index.html
├── css/
│   └── orbent.css
└── assets/
├── logo/
│   ├── logo-corporativa.png
│   ├── orbent-logo-claro.png
│   ├── orbent-logo-escuro.png
│   ├── logo-slogan.png
│   ├── orbent-icon-escuro.png
│   └── orbent-icon-transparente.png
├── pattern/
│   ├── pattern.png
│   ├── pattern_opacidade.png
│   ├── Pattern-galaxia.png
│   └── Hero Section.jpeg
└── palette.png



---

## 🎨 Paleta de Cores

| Nome | Hex | Aplicação |
|------|------|------------|
| **Azul Orbent** | `#001434` | Cor principal / fundo |
| **Azul Acento** | `#5271FF` | Interações e links |
| **Dourado Orbent** | `#CCA300` | Destaques e detalhes premium |
| **Branco Gelo** | `#FDFDFD` | Fundos claros |
| **Cinza Neutro** | `#6B7280` | Texto auxiliar |

![Paleta Orbent](./assets/palette.png)

---

## 🧩 Uso rápido do CSS

### 1️⃣ Importar fontes e estilo base
html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Poppins:wght@600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="./css/orbent.css">


### 2️⃣ Aplicar tema

html
<body class="theme-light">
  <h1 class="gradient-orbent">Orbent</h1>
  <p class="subtitle">Visão sistêmica. Cultura viva. Inteligência com propósito.</p>
</body>


---

## 💫 Gradiente Oficial

css
linear-gradient(45deg, #f8ad00 0%, #e13333 50%, #3992ff 100%);


Aplicação sugerida:

html
<h1 class="gradient-orbent">Orbent</h1>


---

## 🧠 Design System (orbent.css)

### Componentes disponíveis

| Tipo            | Classe                                          | Descrição                |
| --------------- | ----------------------------------------------- | ------------------------ |
| Botão principal | `.btn`                                          | Azul Orbent padrão       |
| Botão gradiente | `.btn--gradient`                                | Gradiente institucional  |
| Cartão          | `.card`                                         | Bloco com sombra e borda |
| Alerta          | `.alert` / `.alert--success` / `.alert--danger` | Mensagens de status      |
| Tabela          | `.table`                                        | Layout básico de dados   |
| Indicador       | `.badge` / `.badge--gold`                       | Status visual            |
| Tema            | `.theme-light` / `.theme-dark`                  | Modos claro e escuro     |

---

## 🧱 Layout de Demonstração

O repositório inclui um arquivo **`index.html`** com o layout **corporativo minimalista**:

html
<body>
  <main class="layout">
    <div class="brand">
      <img src="./assets/logo/logo-corporativa.png" alt="Logo Orbent" />
    </div>
    <div class="slogan">
      Visão sistêmica. <span>Cultura viva.</span><br>Inteligência com propósito.
    </div>
  </main>
</body>


![Exemplo Hero](./assets/pattern/Hero%20Section.jpeg)

---

## 🪶 Patterns e Texturas

| Arquivo                 | Uso                |
| ----------------------- | ------------------ |
| `pattern.png`           | Fundo padrão       |
| `pattern_opacidade.png` | Fundo translúcido  |
| `Pattern-galaxia.png`   | Hero institucional |
| `Hero Section.jpeg`     | Capa promocional   |

---

## ⚙️ White Label

O Design System suporta variações de marca mantendo o selo **“by Orbent”**.

css
:root.brand-client {
  --orb-primary: #0E3A5B;
  --orb-accent: #00C48C;
  --orb-gold: #FF7A59;
}


html
<span class="brand-ribbon">
  ACME <span class="brand-ribbon__by">by Orbent</span>
</span>


---

## 🧾 Documentação complementar

* [📘 STYLE_GUIDE.md](./STYLE_GUIDE.md) → Diretrizes visuais e proporções do logotipo
* [🧩 CSS_GUIDE.md](./CSS_GUIDE.md) → Tokens, classes e uso técnico

---

## 🧠 Integração com outros projetos

Use este repositório como **submódulo Git** para unificar identidade visual:

bash
git submodule add https://github.com/rosanesouzzza/orbent-brand-assets.git src/assets/orbent


Ou importe o CSS diretamente via URL:

css
@import url("https://raw.githubusercontent.com/rosanesouzzza/orbent-brand-assets/main/css/orbent.css");


---

## 📄 Licença

© **Orbent** — Todos os direitos reservados.
Uso permitido apenas em produtos e clientes licenciados **by Orbent**.
Reprodução, redistribuição ou modificação sem autorização é proibida.


```
