# 📂 Estrutura de Pastas - Guia Rápido

## 📁 Organização Atual

```
Homepage/
│
├── 📁 assets/                  → Todas as imagens
│   ├── 🖼️ fotoperfil.jpg      → Foto do hero section
│   ├── 🖼️ fundoescada.jpg     → Background do site
│   ├── 🖼️ lb.jpg              → Logo (header e footer)
│   └── 🖼️ perfil.jpg          → Foto da seção "Sobre"
│
├── 📄 index.html               → Página principal
├── 📄 projetos.html            → Página de projetos
│
├── 🎨 styles.css               → Estilos principais (reformulado)
├── 🎨 style.css                → Estilos da página de loading (projetos antigo)
│
├── 📖 README.md                → Documentação do projeto
├── 📋 MELHORIAS.md             → Lista de melhorias implementadas
├── 🎯 GUIA_MELHORIAS.html     → Guia visual interativo
│
├── 🚫 .gitignore               → Arquivos ignorados pelo Git
└── 📁 .git/                    → Controle de versão
```

## 🔗 Caminhos das Imagens

### No HTML:
```html
<!-- Logo no Header -->
<img src="assets/lb.jpg" alt="logo">

<!-- Foto de Perfil (Hero) -->
<img src="assets/fotoperfil.jpg" alt="perfil">

<!-- Foto da Seção Sobre -->
<img src="assets/perfil.jpg" alt="foto">

<!-- Logo no Footer -->
<img src="assets/lb.jpg" alt="logo">
```

### No CSS:
```css
/* Background do site */
background: url(assets/fundoescada.jpg);
```

## 📝 Arquivos Principais

### `index.html`
- Página principal do portfólio
- Seções: Hero, Sobre, Contato, Footer
- Usa: `styles.css`

### `projetos.html`
- Página de projetos
- Grid com cards de projetos
- Usa: `styles.css` (variáveis) + estilos inline

### `styles.css`
- Sistema de design completo
- Variáveis CSS (cores, espaçamentos, etc.)
- Responsividade

## 🎨 Onde Adicionar Novas Imagens

1. **Salve a imagem** na pasta `assets/`
2. **Referencie no código:**
   - HTML: `<img src="assets/nome-da-imagem.jpg">`
   - CSS: `background: url(assets/nome-da-imagem.jpg)`

## 🔧 Manutenção

### Para adicionar novo projeto:
Edite `projetos.html` e adicione um novo card:
```html
<div class="projeto-card">
    <span class="status-badge status-concluido">Concluído</span>
    <div class="projeto-icon">
        <i class="bi bi-icon-name"></i>
    </div>
    <h3>Nome do Projeto</h3>
    <p>Descrição do projeto...</p>
    <div class="projeto-tags">
        <span class="tag">Tecnologia 1</span>
        <span class="tag">Tecnologia 2</span>
    </div>
    <div class="projeto-links">
        <a href="#" class="projeto-btn">
            <i class="bi bi-eye"></i> Ver Projeto
        </a>
    </div>
</div>
```

### Para alterar cores:
Edite as variáveis em `styles.css` (linhas 1-50):
```css
:root {
    --primary-color: #007bff;    /* Mude aqui */
    --accent-color: #00d4ff;     /* Mude aqui */
}
```

### Para otimizar imagens:
1. Use ferramentas online: TinyPNG, Squoosh
2. Formatos recomendados:
   - `.jpg` para fotos
   - `.png` para logos com transparência
   - `.webp` para melhor compressão (moderna)

## 📱 Testando Responsividade

**No navegador:**
1. Pressione `F12` (DevTools)
2. Clique no ícone de dispositivo móvel
3. Teste diferentes tamanhos:
   - 1920px (Desktop)
   - 1024px (Tablet landscape)
   - 768px (Tablet portrait)
   - 375px (Mobile)

## 🚀 Deploy

### GitHub Pages:
1. Commit e push das alterações
2. Vá em Settings → Pages
3. Selecione branch `main` → pasta `/root`
4. Salve e aguarde deploy

### Netlify/Vercel:
1. Conecte o repositório
2. Deploy automático a cada commit

## 💡 Dicas

- ✅ Sempre teste após adicionar imagens
- ✅ Use nomes descritivos para imagens
- ✅ Comprima imagens antes de adicionar
- ✅ Mantenha backup das imagens originais
- ✅ Commit frequente com mensagens claras

---

**Última atualização:** Fevereiro 2026
