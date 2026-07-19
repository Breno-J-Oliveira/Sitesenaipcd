# ♿ SENAI PCD — Portal de Acessibilidade e Inclusão

<p align="center">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-10B981?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Exibi%C3%A7%C3%A3o-Oficial%20SENAI-2563EB?style=for-the-badge" alt="Exibição SENAI">
  <img src="https://img.shields.io/badge/Foco-Acessibilidade-7C3AED?style=for-the-badge" alt="Acessibilidade">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/WCAG_2.1-Diretrizes-111827?style=for-the-badge" alt="WCAG 2.1">
  <img src="https://img.shields.io/badge/Font_Awesome-528DD7?style=for-the-badge&logo=fontawesome&logoColor=white" alt="Font Awesome">
</p>

---

## 📑 Índice

1. [Sobre o Projeto](#-sobre-o-projeto)
2. [Funcionalidades de Acessibilidade](#-funcionalidades-de-acessibilidade)
3. [Estrutura do Site](#-estrutura-do-site)
4. [Design Inclusivo](#-design-inclusivo)
5. [Recursos Implementados](#-recursos-implementados)
6. [Tecnologias](#-tecnologias)
7. [Contatos](#-contatos)

---

## 🎯 Sobre o Projeto

O **SENAI PCD** é um portal web desenvolvido com foco total em **acessibilidade e inclusão** para Pessoas com Deficiência (PCD). O projeto foi **selecionado para exibição oficial no SENAI** como referência de boas práticas em design inclusivo.

O site aborda temas fundamentais como direitos trabalhistas, vagas de emprego inclusivas, empresas parceiras e recursos de acessibilidade digital — tudo seguindo as diretrizes **WCAG 2.1** (Web Content Accessibility Guidelines).

### 🏆 Reconhecimento
- ✅ **Escolhido para exibição oficial no SENAI**
- ✅ Referência de acessibilidade web na instituição
- ✅ Design seguindo padrões internacionais (WCAG 2.1)

---

## ♿ Funcionalidades de Acessibilidade

| Funcionalidade | Implementação | Diretriz WCAG |
|---------------|---------------|---------------|
| **Alto Contraste** | Fundo escuro com texto branco/amarelo de alto contraste | 1.4.3 (Contraste Mínimo) |
| **Ícones de Acessibilidade** | Botão fixo de Libras e PCD no canto da tela | 3.2.3 (Navegação Consistente) |
| **Textos Alternativos** | Atributos `alt` descritivos em todas as imagens | 1.1.1 (Conteúdo Não Textual) |
| **Navegação por Teclado** | Links e botões acessíveis via `tab` | 2.1.1 (Teclado) |
| **Estrutura Semântica** | Uso correto de `header`, `main`, `aside`, `footer` | 1.3.1 (Info e Relações) |
| **Fontes Legíveis** | Tamanhos adequados, sem serifa, espaçamento generoso | 1.4.4 (Redimensionar Texto) |
| **Tooltips Informativos** | Dicas visuais em CSS puro ao passar o mouse | 3.3.2 (Rótulos ou Instruções) |
| **Layout Responsivo** | Adapta-se a qualquer dispositivo | 1.4.10 (Reflow) |
| **Ícones Aumentados** | Botões de acessibilidade com tamanho ampliado | 2.5.5 (Tamanho do Alvo) |
| **Links Descritivos** | Texto dos links explica o destino | 2.4.4 (Finalidade do Link) |

---

## 🏗️ Estrutura do Site

```
<body>
  <header>
    ✅ Logo SENAI
    ✅ Ícones fixos de acessibilidade (Libras e PCD)
  </header>

  <main>
    ✅ Hero Banner — "Vagas para PCD"
    ✅ Seção de Vagas de Emprego (cards)
    ✅ Seção de Empresas Parceiras (logos)
    ✅ Seção de Direitos Trabalhistas
  </main>

  <aside>
    ✅ Sidebar com informações complementares
  </aside>

  <footer>
    ✅ Links institucionais
    ✅ Informações de contato
  </footer>
</body>
```

### Ícones de Acessibilidade

O site implementa **ícones fixos** (posicionamento `fixed`) que permanecem visíveis durante toda a navegação:

- **Ícone de Libras:** Acesso a conteúdo em Língua Brasileira de Sinais
- **Ícone PCD:** Acesso rápido a funcionalidades de acessibilidade

```css
.icone-libras, .icone-pcd {
  position: fixed;
  right: 20px;
  z-index: 1000;
  background: #7C3AED;
  color: white;
  padding: 12px;
  border-radius: 50%;
  cursor: pointer;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}
```

### Empresas Parceiras (Logos com Tooltips)

O site exibe logos de empresas parceiras com **tooltips CSS puro**:

| Empresa | Logo |
|---------|------|
| Serasa Experian | `sl.png` |
| Bradesco | `bradesco.png` |
| Habib's | `habibs.png` |

---

## 🎨 Design Inclusivo

### Princípios Aplicados

1. **Perceptível:** Informações visíveis para todos os utilizadores
2. **Operável:** Interface navegável por teclado e mouse
3. **Compreensível:** Conteúdo claro e previsível
4. **Robusto:** Compatível com leitores de ecrã

### Paleta de Alto Contraste

| Elemento | Cor | Contraste |
|----------|-----|-----------|
| Fundo Principal | `#1a1a2e` (azul escuro) | - |
| Fundo Secundário | `#16213e` | - |
| Texto Principal | `#ffffff` (branco) | 15.2:1 ✅ |
| Destaques | `#e94560` (vermelho) | 5.8:1 ✅ |
| Links | `#0f3460` com underline | - |

---

## 📁 Arquivos Principais

| Arquivo | Linhas | Descrição |
|---------|--------|-----------|
| `index.html` | 142 | Página principal com todas as seções |
| `style.css` | 298 | CSS completo com design system |
| `assets/Pictures/` | 7 imagens | Logos, banner, ícones |

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|-----------|-----|
| **HTML5** | Estrutura semântica acessível |
| **CSS3** | Flexbox, posicionamento fixo, tooltips, animações |
| **Font Awesome 7.0.1** | Ícones vetoriais (CDN) |
| **WCAG 2.1** | Diretrizes de acessibilidade |


## 👤 Contatos e Redes Sociais

<p align="center">
  <a href="https://github.com/Breno-J-Oliveira" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/breno-j-oliveira-672619352/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://www.instagram.com/brenoov" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
  <a href="https://x.com/BrenoJOliveira_" target="_blank">
    <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X (Twitter)">
  </a>
</p>

---

<p align="center"><em>Desenvolvido com 💛 por Breno Oliveira — Técnico em Desenvolvimento de Sistemas | SENAI</em></p>
