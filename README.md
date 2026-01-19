# Snitap Patins — Landing Page com animações em CSS

Landing page estática criada no contexto do curso da Rocketseat (**Bases do Front-end / aula de CSS**), explorando **animações e interações usando apenas HTML + CSS**.

## ✨ Demonstração / Deploy

- **Deploy (Netlify)**: https://patins-animation.netlify.app/
- Abra `index.html` no navegador ou rode um servidor local (recomendado) para evitar problemas de caminhos.

## ✅ Funcionalidades

- **Hero animado**
  - Entrada (slide-in) dos elementos visuais (círculo, patins e estrelas)
  - Título com **palavras rotativas** (animação de “slide up”)
- **Banner infinito**
  - Rolagem horizontal contínua
  - Gradiente com animação suave
- **Galeria**
  - Grid responsivo de imagens
  - Hover com zoom e legenda
  - Aparição na rolagem (scroll-driven animation, quando suportado)
- **Header/Footer**
  - Micro-interações (rotações no hover, underline animado, highlight nos ícones sociais)

## 🧪 Tecnologias

- **HTML5**
- **CSS3**

## ▶️ Como executar

### Opção 1 — Abrir diretamente

- Abra o arquivo `index.html` no navegador.

> Observação: em alguns ambientes, abrir “direto do arquivo” pode impactar caminhos. Se algo não carregar, use um servidor local (opções abaixo).

### Opção 2 — VS Code (Live Server)

- Instale a extensão **Live Server**
- Clique com o botão direito no `index.html` → **Open with Live Server**

### Opção 3 — Servidor simples via Node (sem instalar dependências no projeto)

No terminal, dentro da pasta do projeto:

```bash
npx serve .
```

Depois, acesse a URL exibida no terminal.

## 🗂️ Estrutura de pastas

```text
.
├─ index.html
├─ styles/
│  ├─ index.css        # importa os módulos (global/header/hero/banner/gallery/footer)
│  ├─ global.css
│  ├─ header.css
│  ├─ hero.css
│  ├─ banner.css
│  ├─ gallery.css
│  └─ footer.css
└─ assets/
   ├─ logo.svg
   ├─ banner.svg
   ├─ hero/            # imagens do hero (patins, estrelas, ellipse)
   ├─ icons/
   └─ images/          # imagens da galeria
```

## 🎛️ Onde mexer (guia rápido)

- **Estilos globais e variáveis**: `styles/global.css`
- **Header (badge e hover)**: `styles/header.css`
- **Hero**
  - Animações: `styles/hero.css` (`@keyframes slideIn`, `appear`, `slideUp`)
  - Conteúdo: `index.html` (seção `.hero`)
- **Banner infinito**: `styles/banner.css` (`@keyframes rolling`, `bg-gradient`)
- **Galeria**: `styles/gallery.css` (`@keyframes image-appear`)
- **Footer e links sociais**: `styles/footer.css`

## ⚠️ Compatibilidade (importante)

Em `styles/gallery.css`, a animação baseada em rolagem usa:

- `animation-timeline: view()`
- `animation-range: ...`

Esses recursos podem **não funcionar em todos os navegadores**. O layout e o hover continuam funcionando normalmente; apenas a animação “on scroll” pode não acontecer dependendo do suporte do navegador.

## 📸 Capturas

> Adicione suas imagens na pasta `assets/` e referencie-as aqui. Sugestão de nomes:
>
> - `assets/preview-home.png` (hero + banner)
> - `assets/preview-gallery.png` (galeria)
>
> Exemplo de uso em Markdown (após adicionar os arquivos):
>
> ```md
> ![Preview hero](assets/preview-home.png)
> ![Preview galeria](assets/preview-gallery.png)
> ```

## 📌 Créditos

- Projeto desenvolvido a partir de aulas da **Rocketseat** (trilha Bases do Front-end).

## 📄 Licença

Este repositório não declara uma licença. Se você quiser abrir para uso/redistribuição, adicione um arquivo `LICENSE` (por exemplo, MIT).

