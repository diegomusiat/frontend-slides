# RD Medicine — Presentation Redesign Brief
**Para uso no Claude Code | HTML/CSS/JS — Single File**

---

## Visão Geral

Recriar a apresentação "RD Medicine: O Próximo Nível" como uma **landing page de apresentação interativa** (substituto moderno de slides), mantendo 100% do conteúdo original mas com uma diagramação editorial, sofisticada e memorável — digna de um pitch de brand strategy de alto nível.

---

## Direção Estética

**Conceito: "Editorial de Luxo Institucional"**

Inspiração: anuário de arquitetura, relatório anual de consultoria top-tier (McKinsey, Interbrand), editorial de medicina de prestígio.

- **Tema:** Dark elegante — fundo `#0A0D14` (quase preto azulado) com elementos em branco e dourado
- **Tipografia:**
  - Display/Títulos: `Playfair Display` (Google Fonts) — serifado, peso 700/900
  - Corpo/Labels: `DM Sans` (Google Fonts) — peso 300/400/600
  - Accent/Quotes: `DM Serif Display` em itálico para citações
- **Paleta:**
  - `#0A0D14` — fundo principal
  - `#FFFFFF` — texto primário
  - `#C9A96E` — dourado accent (substitui o laranja original)
  - `#1A2035` — cards/superfícies elevadas
  - `#2A3A5C` — borda/divisor sutil
  - `#E8E8E8` — texto secundário
- **Motion:** Fade + slide-up ao entrar no viewport (Intersection Observer). Progress bar no topo. Sem animações excessivas — peso e autoridade.

---

## Estrutura da Página

A apresentação é uma **página vertical contínua** dividida em **12 seções**, navegáveis por um **menu lateral fixo** (dot navigation) + scroll natural.

### Navegação
- Barra lateral direita com dots numerados (01–12)
- Ao hover: tooltip com nome da seção
- Dot ativo destaca em dourado
- Header fixo minimalista com logo "RD Medicine" à esquerda e "Ciclo Estratégico 12 Meses" à direita

---

## Seções e Diagramação

### SEÇÃO 01 — Hero / Capa
**Conteúdo original:** Título principal + subtítulo + tagline

**Nova diagramação:**
- Full viewport height (`100vh`)
- Fundo com mesh gradient sutil animado (CSS `@keyframes`) em tons de azul escuro
- Título "RD MEDICINE:" em Playfair Display, tamanho gigante (clamp 64px–120px), quebrando em 2 linhas com efeito de reveal por letras (JS simples)
- Subtítulo "O PRÓXIMO NÍVEL" em DM Sans bold, espaçamento de letras largo, cor branca
- Abaixo: linha dourada horizontal (`2px`, `80px` de largura) como divisor decorativo
- "Construção de Brand Equity e Crescimento Sustentável" em DM Sans 300, cinza claro
- "CICLO ESTRATÉGICO DE 12 MESES" em dourado, uppercase, tracking largo, letra pequena
- Canto inferior direito: seta animada indicando scroll

---

### SEÇÃO 02 — Crescer Rápido Exige Sustentação Estratégica
**Conteúdo original:** 4 pontos + citação

**Nova diagramação:**
- Layout dividido: esquerda 40% com título grande + citação em destaque; direita 60% com os 4 pontos
- Cada ponto: numerado com `01 / 02 / 03 / 04` em dourado à esquerda, texto à direita, separados por linha sutil
- A citação em bloco: fundo `#1A2035`, borda esquerda dourada (`4px`), texto em Playfair Display itálico, tamanho grande
- Background da seção: sutil ruído/grain overlay via CSS

---

### SEÇÃO 03 — Metodologia Brand for Equity
**Conteúdo original:** 4 fases (Leitura, Ativos, Ativação, Governança)

**Nova diagramação:**
- Título + subtítulo no topo, centralizados
- Abaixo: 4 cards em grid horizontal `repeat(4, 1fr)`
- Cada card:
  - Número grande (01–04) em Playfair Display, 80px, semi-transparente (dourado 20% opacity) no background do card
  - Ícone SVG minimalista no topo (relacionado ao tema de cada fase)
  - Título em maiúsculas, DM Sans 600
  - Texto descritivo em DM Sans 300
  - Borda superior dourada que "preenche" de 0 a 100% no hover (CSS transition)
- Footer da seção: citação em destaque, centralizada, Playfair itálico

---

### SEÇÃO 04 — Liderança Executiva: Sandro Serzedello
**Conteúdo original:** 3 bullets de atributos + citação + texto principal

**Nova diagramação:**
- Layout assimétrico: coluna esquerda 55% com texto; coluna direita 45% com elemento visual abstrato (círculo com gradiente dourado + "Brand Equity Constructor" como texto circular animado via SVG)
- "Brand Equity Constructor" como label em dourado, uppercase
- Os 3 bullets transformados em 3 "pilares" verticais com linha divisória entre eles
- Citação no rodapé da seção, full-width, fundo levemente diferenciado

---

### SEÇÃO 05 — Liderança Integrada e Alinhamento Executivo
**Conteúdo original:** BOARD, MARKETING, AGÊNCIA, PR & ASSESSORIA + citação

**Nova diagramação:**
- Diagrama visual de hierarquia/spoke:
  - Centro: círculo com "SANDRO SERZEDELLO" 
  - 4 nós ao redor conectados por linhas: BOARD / MARKETING / AGÊNCIA / PR & ASSESSORIA
  - Cada nó: círculo com label + ao hover expande para mostrar o texto descritivo
  - Implementado em SVG puro + CSS hover
- Título e citação fora do diagrama, acima e abaixo

---

### SEÇÃO 06 — Ecossistema RD
**Conteúdo original:** 4 entidades (RD Medicine, RD Residência, Rafael Duarte, Rute Duarte)

**Nova diagramação:**
- Título "ECOSSISTEMA RD" centralizado com subtítulo "Sincronia entre Institucional, Produto e Pessoal"
- 4 cards em grid 2×2
- Cada card com fundo `#1A2035`, hover eleva com `box-shadow` dourado
- Ícone SVG diferente para cada entidade (institucional, produto, pessoa, pessoa)
- Tag role em dourado uppercase
- Texto descritivo em cinza claro
- Footer da seção: citação "4 motores operando como um sistema único..."

---

### SEÇÃO 07 — LABrand: O Cérebro da Operação
**Conteúdo original:** 4 capacidades + "Ativação Imediata"

**Nova diagramação:**
- Fundo diferenciado: `#0D1120` com grid de pontos decorativo (CSS background-image)
- Lado esquerdo: texto "Ativação Imediata" + parágrafo + as 4 capacidades como lista estilizada (ícone + título bold + descrição)
- Lado direito: mockup de dashboard desenhado em HTML/CSS (sem imagem) — janela de browser estilizada com elementos fictícios simulando o LABrand dashboard (sidebar com itens, área de conteúdo com cards de progresso)
- Citação no rodapé

---

### SEÇÃO 08 — Roadmap Semestre 01
**Conteúdo original:** Onda 1 (Meses 1-3) + Onda 2 (Meses 4-6)

**Nova diagramação:**
- Timeline horizontal com linha dourada conectando os 6 meses
- Cada mês: círculo numerado na linha + card acima/abaixo alternando (zig-zag)
- Onda 1 (meses 1-3): cards em tom azul-escuro com badge "FUNDAÇÃO"
- Onda 2 (meses 4-6): cards em tom ligeiramente mais claro com badge "CONSTRUÇÃO"
- Resultado esperado de cada onda: box destacado com borda dourada no topo
- Citação no rodapé

---

### SEÇÃO 09 — Roadmap Semestre 02
**Conteúdo original:** Onda 3 (Meses 7-9) + Onda 4 (Meses 10-12)

**Nova diagramação:**
- Mesma lógica da Seção 08, continuidade visual
- Onda 3: badge "ATIVAÇÃO"
- Onda 4: badge "GOVERNANÇA"
- A linha da timeline é contínua visualmente com a seção anterior (sem divisor brusco)

---

### SEÇÃO 10 — Ativos Estratégicos Que Ficam na Empresa
**Conteúdo original:** 4 grupos de entregáveis

**Nova diagramação:**
- Grid 2×2 de cards grandes
- Cada card tem:
  - Cor de borda esquerda distinta (dourado, azul médio, branco, verde-azulado)
  - Título do grupo em uppercase, DM Sans 600
  - Lista dos entregáveis com marcador `→` em dourado
  - Ícone SVG no canto superior direito do card
- Footer: citação full-width destacada

---

### SEÇÃO 11 — O Compromisso do Sucesso
**Conteúdo original:** DECISORES, DADOS, INTERFACE, FOCO

**Nova diagramação:**
- Fundo full-width com gradiente sutil direcional (mais escuro nas bordas)
- Título centralizado com subtítulo em dourado
- 4 itens em layout horizontal, cada um:
  - Número romano (I, II, III, IV) em dourado grande como decoração
  - Label em uppercase bold
  - Texto descritivo
  - Separados por linha vertical `1px` dourada
- Citação centralizada embaixo

---

### SEÇÃO 12 — CTA Final / Próximos Passos
**Conteúdo original:** Pergunta retórica + 4 próximos passos

**Nova diagramação:**
- Full viewport height
- Pergunta "CONSTRUIR ATIVO OU APENAS COMPRAR CRESCIMENTO?" em Playfair Display gigante, centralizada, com "CRESCIMENTO?" em dourado
- Parágrafo justificativo em DM Sans 300
- Os 4 próximos passos em lista numerada estilizada, cada item com animação de entrada escalonada
- Botão/elemento CTA: "INICIAR O CICLO" — botão com borda dourada, hover preenche de dourado, texto muda para preto
- Footer mínimo: "RD Medicine × Sandro Serzedello | Ciclo Estratégico 12 Meses"

---

## Detalhes Técnicos

```
Arquivo único: index.html
Fontes: Google Fonts (Playfair Display, DM Sans, DM Serif Display)
Sem frameworks externos (vanilla HTML/CSS/JS)
JS mínimo para: dot nav, Intersection Observer (scroll reveal), timeline interativa
CSS: variáveis, grid, flexbox, animações com keyframes
Responsivo: ≥ 768px (foco em desktop, mobile adequado)
```

### CSS Variables a definir:
```css
:root {
  --bg-primary: #0A0D14;
  --bg-surface: #1A2035;
  --bg-elevated: #222B42;
  --accent-gold: #C9A96E;
  --accent-gold-dim: rgba(201, 169, 110, 0.15);
  --text-primary: #FFFFFF;
  --text-secondary: #A0AABF;
  --text-muted: #5A6480;
  --border-subtle: #2A3A5C;
  --font-display: 'Playfair Display', serif;
  --font-body: 'DM Sans', sans-serif;
  --font-quote: 'DM Serif Display', serif;
}
```

### Scroll Reveal (JS):
```javascript
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
    }
  });
}, { threshold: 0.15 });

document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
```

### CSS Reveal:
```css
.reveal {
  opacity: 0;
  transform: translateY(32px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}
.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}
.reveal-delay-1 { transition-delay: 0.1s; }
.reveal-delay-2 { transition-delay: 0.2s; }
.reveal-delay-3 { transition-delay: 0.3s; }
```

### Progress Bar:
```css
#progress-bar {
  position: fixed;
  top: 0;
  left: 0;
  height: 2px;
  background: var(--accent-gold);
  z-index: 1000;
  transition: width 0.1s linear;
}
```

---

## O Que NÃO Fazer

- ❌ Não usar fundo branco
- ❌ Não usar Inter, Roboto ou Arial
- ❌ Não usar gradientes roxos/violeta
- ❌ Não replicar o layout dos slides originais (colunas com borda azul simples)
- ❌ Não usar imagens externas (apenas SVGs inline e CSS shapes)
- ❌ Não usar bibliotecas de terceiros (sem Bootstrap, Tailwind, etc.)
- ❌ Não omitir nenhum conteúdo textual original

---

## Checklist Final

- [ ] Todos os 12 conteúdos das seções presentes e completos
- [ ] Tipografia Playfair Display + DM Sans aplicada corretamente
- [ ] Paleta dark/dourada consistente em todo o documento
- [ ] Dot navigation lateral funcional com highlight ativo
- [ ] Scroll reveal funcionando em todos os elementos `.reveal`
- [ ] Progress bar de leitura no topo
- [ ] Diagrama spoke da Seção 05 funcional em SVG+CSS
- [ ] Timeline das Seções 08 e 09 visualmente conectada
- [ ] Mockup de dashboard HTML/CSS na Seção 07
- [ ] Responsividade básica ≥ 768px
- [ ] Nenhuma dependência externa além do Google Fonts
