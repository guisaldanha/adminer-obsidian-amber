<div align="center">

# 🟠 Obsidian Amber
### Um tema escuro e refinado para o [Adminer](https://www.adminer.org/)

[![License: MIT](https://img.shields.io/badge/License-MIT-f59e0b?style=flat-square)](LICENSE)
[![Adminer](https://img.shields.io/badge/Adminer-5.x-10b981?style=flat-square)](https://www.adminer.org/)
[![CSS](https://img.shields.io/badge/Pure-CSS-58a6ff?style=flat-square)](#)
[![Autor](https://img.shields.io/badge/Autor-Guilherme%20Saldanha-f59e0b?style=flat-square)](https://guisaldanha.com)

</div>

---

## ✨ Visão Geral

**Obsidian Amber** é um tema dark para o Adminer com estética de terminal futurista. Combina o fundo profundo do Obsidian com acentos em âmbar dourado e esmeralda, tipografia monospace premium e ícones SVG inline — tudo em um único arquivo CSS, sem dependências externas além das fontes do Google Fonts.

### Paleta de cores

| Papel | Cor | Hex |
|-------|-----|-----|
| Fundo principal | ![#0d1117](https://placehold.co/14x14/0d1117/0d1117.png) Obsidian | `#0d1117` |
| Fundo secundário | ![#161b22](https://placehold.co/14x14/161b22/161b22.png) Obsidian 2 | `#161b22` |
| Acento primário | ![#f59e0b](https://placehold.co/14x14/f59e0b/f59e0b.png) Âmbar | `#f59e0b` |
| Acento secundário | ![#10b981](https://placehold.co/14x14/10b981/10b981.png) Esmeralda | `#10b981` |
| Texto principal | ![#e6edf3](https://placehold.co/14x14/e6edf3/e6edf3.png) Ice | `#e6edf3` |
| Erro / Destaque | ![#f87171](https://placehold.co/14x14/f87171/f87171.png) Coral | `#f87171` |

### Tipografia

- **Corpo:** [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) — monospace premium para leitura de dados
- **Títulos:** [Syne](https://fonts.google.com/specimen/Syne) — display geométrica moderna

---

## 🚀 Instalação

### 1. Baixe o arquivo

```bash
curl -o adminer.css https://raw.githubusercontent.com/guisaldanha/adminer-obsidian-amber/main/adminer.css
```

Ou clone o repositório:

```bash
git clone https://github.com/guisaldanha/adminer-obsidian-amber.git
```

### 2. Coloque no mesmo diretório do Adminer

```
seu-projeto/
├── adminer-5.x.x.php   ← arquivo do Adminer
└── adminer.css          ← tema Obsidian Amber ✅
```

### 3. Pronto!

O Adminer detecta automaticamente qualquer arquivo `adminer.css` na mesma pasta e o aplica. Não é necessário nenhuma configuração adicional.

---

## 📦 O que está incluído

| Recurso | Detalhe |
|---------|---------|
| 🎨 Tema dark completo | Todos os 133 seletores do Adminer estilizados |
| 🖼️ Ícones SVG inline | `icon-up`, `icon-down`, `icon-plus`, `icon-cross`, `icon-move` e mais |
| 🌈 Syntax highlighting | Esquema de cores Obsidian para o JUSH (SQL, PHP, HTML, JS, CSS) |
| 📱 Responsivo | Adaptado para mobile com `@media (max-width: 800px)` |
| 🖨️ Print-friendly | Estilos específicos para impressão em `@media print` |
| ↔️ Suporte RTL | Compatível com layouts da direita para esquerda |
| 🔤 Fontes via Google Fonts | JetBrains Mono + Syne (requer conexão à internet) |
| 🖱️ Menu inteligente | Nomes de tabelas longos expandem individualmente no hover |

---

## ⚙️ Uso offline (fontes locais)

Por padrão, o tema carrega as fontes via Google Fonts. Se precisar de uso 100% offline:

1. Baixe as fontes:
   - [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono)
   - [Syne](https://fonts.google.com/specimen/Syne)

2. Coloque os arquivos `.woff2` em uma pasta `fonts/` ao lado do `adminer.css`

3. Substitua o `@import` no início do CSS:

```css
/* Remova esta linha: */
@import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono...');

/* Adicione estas: */
@font-face {
    font-family: 'JetBrains Mono';
    src: url('fonts/JetBrainsMono-Regular.woff2') format('woff2');
    font-weight: 400;
}
@font-face {
    font-family: 'Syne';
    src: url('fonts/Syne-Regular.woff2') format('woff2');
    font-weight: 400;
}
/* ... demais pesos conforme necessário */
```

---

## 🔧 Customização

Todas as cores e variáveis ficam no topo do arquivo na seção `:root` / `html`. Para mudar o acento principal de âmbar para outra cor, basta alterar as variáveis:

```css
html {
    --amber:     #f59e0b;   /* cor de destaque principal */
    --amber-dim: #78350f;   /* versão escura do destaque */
    --emerald:   #10b981;   /* cor de destaque secundária */
}
```

---

## 🧪 Compatibilidade

| Adminer | Compatível |
|---------|-----------|
| 5.x     | ✅ Testado |
| 4.x     | ✅ Deve funcionar |
| 3.x     | ⚠️ Não testado |

| Banco de dados | Compatível |
|----------------|-----------|
| MySQL / MariaDB | ✅ |
| PostgreSQL | ✅ |
| SQLite | ✅ |
| MS SQL Server | ✅ |
| Oracle | ✅ |

---

## 📄 Licença

Distribuído sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

```
MIT License — Copyright (c) 2026 Guilherme Saldanha
```

---

## 👤 Autor

**Guilherme Saldanha**

- 🌐 [guisaldanha.com](https://guisaldanha.com)
- 🐙 GitHub: [@guisaldanha](https://github.com/guisaldanha)

---

<div align="center">

Feito com ☕ e muitas linhas de CSS

Se este tema foi útil para você, considere dar uma ⭐ no repositório!

</div>