# Bikcraft

![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

> Landing page institucional de bicicletas elétricas personalizadas, com foco em design moderno, acessibilidade e experiência do usuário.

[🔗 Ver Demo](https://lucascastilhodev.github.io/bikcraft/)

---

## Sobre o Projeto

Bikcraft é uma landing page institucional de bicicletas elétricas customizadas, desenvolvida como projeto de conclusão do curso **HTML e CSS para Iniciantes** da [Origamid](https://www.origamid.com/).

O design e UI/UX foram criados pela Origamid, enquanto toda a implementação do código (HTML, CSS e JavaScript) foi realizada por mim, aplicando as melhores práticas de desenvolvimento web moderno, com foco em semântica, responsividade e acessibilidade.

### Funcionalidades

- Página inicial com apresentação de produtos e serviços
- Catálogo de bicicletas com três modelos (Nimbus Stark, Magic Might, Nebula Cosmic)
- Páginas individuais para cada modelo com galeria interativa
- Planos de seguro (Prata e Ouro) com comparativo de benefícios
- Sistema de orçamento com formulário dinâmico
- Página de contato com formulário e localização das lojas
- FAQ com accordion interativo
- Animações suaves com scroll reveal

---

## Características Técnicas

### HTML Semântico
- Estrutura semântica com tags apropriadas (`<header>`, `<main>`, `<article>`, `<section>`)
- Atributos ARIA para acessibilidade
- Meta tags otimizadas para SEO

### CSS Modular
- **Arquitetura**: Organização modular por componentes e páginas
- **CSS Grid & Flexbox** para layouts responsivos
- **CSS Variables** para gerenciamento de cores e tokens de design
- **Mobile-first** com breakpoints em 400px, 600px e 800px
- **Tipografia** customizada com Google Fonts (Poppins, Roboto, Merriweather)

### JavaScript Vanilla
- **Navegação ativa**: Destaque automático da página atual no menu
- **Galeria interativa**: Troca de imagens ao clicar (desktop)
- **Accordion FAQ**: Sistema de perguntas e respostas expansível
- **Formulário inteligente**: Preenchimento automático via URL params
- **Animações**: Integração com biblioteca SimpleAnime para scroll reveal

---

## Estrutura de Arquivos

```
bikcraft/
├── index.html
├── bicicletas.html
├── seguros.html
├── contato.html
├── orcamento.html
├── termos.html
├── bicicletas/
│   ├── nimbus.html
│   ├── magic.html
│   └── nebula.html
├── css/
│   ├── style.css
│   ├── global/
│   │   ├── global.css
│   │   ├── header.css
│   │   └── footer.css
│   ├── utilidades/
│   │   ├── componentes.css
│   │   ├── cores.css
│   │   ├── tipografia.css
│   │   ├── formulario.css
│   │   └── animacao.css
│   ├── home/
│   ├── bicicletas/
│   ├── seguros/
│   ├── contato/
│   └── orcamento/
├── js/
│   ├── script.js
│   └── plugins/
│       └── simple-anime.js
└── img/
```

---

## Como Executar

### Pré-requisitos
- Navegador web moderno
- Editor de código (recomendado: VSCode)
- Live Server (opcional)

### Instalação

1. **Clone o repositório**
```bash
git clone https://github.com/LucasCastilhoDev/bikcraft.git
```

2. **Navegue até a pasta**
```bash
cd bikcraft
```

3. **Abra com Live Server**
   - No VSCode: Clique com botão direito no `index.html` → "Open with Live Server"
   - Ou simplesmente abra o `index.html` no navegador

---

## Destaques do Código

### Sistema de Cores com CSS Variables
```css
:root {
  --cor-0: #ffffff;
  --cor-11: #111111;
  --cor-12: #000000;
  --cor-p1: #ffbb00;
  /* ... */
}
```

### Grid Responsivo
```css
.bicicletas {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
}

@media (max-width: 800px) {
  .bicicletas {
    grid-template-columns: 1fr;
  }
}
```

### Accordion Interativo
```javascript
function ativarPergunta(event) {
  const pergunta = event.currentTarget;
  const controls = pergunta.getAttribute("aria-controls");
  const resposta = document.getElementById(controls);
  resposta.classList.toggle("ativa");
}
```

---

## Responsividade

O projeto é totalmente responsivo com breakpoints estratégicos:

- **Desktop**: 1200px+ (layout completo)
- **Tablet**: 800px - 1199px (ajustes de grid)
- **Mobile**: 400px - 799px (layout em coluna única)
- **Mobile Small**: < 400px (ajustes finos)

---

##  Acessibilidade

- Navegação por teclado funcional
- Atributos ARIA (`aria-label`, `aria-controls`, `aria-expanded`)
- Contraste de cores adequado (WCAG AA)
- Textos alternativos em imagens
- Foco visível em elementos interativos

---

##  Design System

### Cores
- **Primária**: Amarelo (#FFBB00)
- **Neutras**: Escala de cinza (12 tons)
- **Background**: Preto (#000000) e Branco (#FFFFFF)

### Tipografia
- **Display**: Poppins (600)
- **Títulos**: Poppins (400-600)
- **Corpo**: Roboto (400-500)
- **Citações**: Merriweather (900 italic)

---

##  Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **CSS3** - Estilização e animações
- **JavaScript (ES6+)** - Interatividade
- **Google Fonts** - Tipografia
- **SimpleAnime.js** - Animações de scroll

---

## 🎓 Aprendizados

Este projeto foi desenvolvido como conclusão do curso **HTML e CSS para Iniciantes** da [Origamid](https://www.origamid.com/), onde apliquei na prática conceitos de:

- Semântica HTML5
- CSS Grid e Flexbox avançado
- Design responsivo mobile-first
- Acessibilidade web (WCAG)
- JavaScript vanilla para interatividade
- Organização modular de código CSS
- Boas práticas de desenvolvimento front-end

**Créditos de Design**: O design e UI/UX são de autoria da Origamid. Minha contribuição foi a implementação completa do código, garantindo fidelidade ao design, responsividade e funcionalidade.

---

##  Licença

Este projeto foi desenvolvido para fins educacionais.

---

##  Autor

**Lucas Castilho**

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-a-castilho/)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/LucasCastilhoDev)
[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:lucasxcastilho@gmail.com)

---
