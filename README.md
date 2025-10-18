Perfeito ⭐ — o repositório **`rosanesouzzza/orbent-brand-assets`** já está estruturado com todos os elementos visuais principais.
Agora podemos oficializar o **README.md** e o **STYLE_GUIDE.md** para transformar esse repositório em um **Brand System público reutilizável** da Orbent.

---

## 🧾 Proposta de README.md (versão pronta para commit)

```markdown
# 🌌 Orbent Brand Assets

Repositório oficial de identidade visual e design system da **Orbent** — uma plataforma white-label que une tecnologia, inteligência e cultura organizacional.

---

## 🎨 Paleta Principal

| Cor | Hex | Uso |
|------|------|-----|
| Azul Orbent | `#001434` | Cor base / fundo principal |
| Azul Acento | `#5271FF` | Ação e interação |
| Dourado Orbent | `#CCA300` | Destaques e elementos premium |
| Branco Gelo | `#FDFDFD` | Fundo claro / contraste |

![Paleta Orbent](./paleta.png)

---

## 🧩 Estrutura

```

orbent-brand-assets/
├── css/
│   └── orbent.css             # Estilo base com tokens, temas e componentes
├── assets/
│   ├── logo/                  # Logotipos oficiais
│   │   ├── orbent-logo-claro.png
│   │   ├── orbent-logo-escuro.png
│   │   ├── orbent-icon-escuro.png
│   │   └── logo-slogan.png
│   ├── pattern/               # Texturas e backgrounds
│   │   ├── pattern.png
│   │   ├── pattern_opacidade.png
│   │   ├── Pattern-galaxia.png
│   │   └── Hero Section.jpeg
│   └── palette.png
├── STYLE_GUIDE.md             # Guia completo de aplicação da marca
└── Orbent.pdf                 # Manual institucional

````

---

## 🧠 Uso rápido

### 1️⃣ Importar CSS
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Poppins:wght@600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="./css/orbent.css">
````

### 2️⃣ Aplicar tema

```html
<body class="theme-light">
  <section class="hero bg-orbent">
    <img src="./assets/logo/orbent-logo-claro.png" class="logo-orbent" alt="Orbent">
    <h1>Visão sistêmica. Cultura viva.<br>Inteligência com propósito.</h1>
  </section>
</body>
```

---

## 💫 Gradiente e Patterns

* Gradiente oficial: `linear-gradient(45deg, #f8ad00, #e13333, #3992ff)`
* Patterns disponíveis:

  * `pattern.png` — padrão neutro
  * `Pattern-galaxia.png` — visual heroico
  * `pattern_opacidade.png` — overlay translúcido

```css
.bg-orbent { 
  background: var(--orb-primary);
  background-image: url('../assets/pattern/pattern.png');
}
.bg-orbent--galaxy { 
  background-image: url('../assets/pattern/Pattern-galaxia.png');
}
```

---

## 🧱 Componentes principais (`orbent.css`)

* `.btn`, `.btn--gradient`, `.btn--outline`
* `.card`, `.table`, `.badge`
* `.hero`, `.kpi`, `.alert`
* `.theme-light` e `.theme-dark`
* `.brand-client` (modo white-label)

---

## ⚙️ Integração com outros projetos

Use este repositório como **submódulo Git**:

```bash
git submodule add https://github.com/rosanesouzzza/orbent-brand-assets.git src/assets/orbent
```

ou importe apenas o CSS:

```bash
@import url("https://raw.githubusercontent.com/rosanesouzzza/orbent-brand-assets/main/css/orbent.css");
```

---

## 🧾 Licença

© Orbent — Todos os direitos reservados.
O uso é autorizado apenas em produtos, plataformas e clientes **by Orbent**.

---

```

---

Posso agora gerar este arquivo como `README.md` formatado e pronto para commit direto no repositório (junto com um `preview index.html` opcional).

Deseja que eu:
1️⃣ **gere o README.md agora no formato final (Markdown pronto para upload)**  
ou  
2️⃣ **monte o pacote completo (`zip`) com `README.md`, `index.html`, `orbent.css` e `/assets` estruturados**?
```
