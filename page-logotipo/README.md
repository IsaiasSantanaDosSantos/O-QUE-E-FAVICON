# Logotipo da Página: Tudo o que Você Precisa Saber

## O que é o Logotipo da Página?

O **logotipo da página** é uma identidade visual exibida na barra de navegação, cabeçalho e rodapé do site. Ele ajuda a reforçar a marca e melhorar a experiência do usuário.

### Exemplos de Locais Onde o Logo Pode Aparecer:

- **Barra de navegação (Header)**
- **Rodapé (Footer)**
- **Página de login**
- **Favicon (ícone da aba do navegador)**

![Exemplo de Logotipo no Site](https://github.com/IsaiasSantanaDosSantos/Pre-delivery-checklist/blob/main/page-logotipo/image/logotipoExemple.png)

---

## Como Adicionar um Logotipo no sistema da DRM?

Clique em "Meu Site":
![Meu Site](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/image/meuSite.png)

Depois clique em "Página Principal":
![Página principal](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/image/mainPage.png)

Depois em "Logotipo e ícone":
![Logotipo e ícone](https://github.com/IsaiasSantanaDosSantos/Pre-delivery-checklist/blob/main/image/faviconDRM.png)

Na lista, clique em "Logotipo (162x60)" e faço o upload de um logo tipo obedecendo as especificações:
![Editar logotipo](https://github.com/IsaiasSantanaDosSantos/Pre-delivery-checklist/blob/main/page-logotipo/image/logotipoEdite.png)

## Pronto!

## Como Adicionar um Logotipo no HTML?

Para inserir um logotipo no site, utilize a tag `<img>` dentro do `<header>` e `<footer>`:

```html
<header>
  <img src="logo.png" alt="Meu Logotipo" width="150" />
</header>
```

No rodapé, pode ser usado da seguinte forma:

```html
<footer>
  <img src="logo.png" alt="Meu Logotipo" width="100" />
</footer>
```

---

## Formatos e Tamanhos Recomendados

Para melhor exibição, utilize os seguintes formatos e tamanhos:  
✅ **PNG** (Fundo transparente recomendado)  
✅ **SVG** (Melhor para escalabilidade e qualidade)  
✅ **JPEG** (Se precisar de imagens mais leves)  
✅ **Tamanho recomendado:** 200x50px (para menus) e 100x100px (para rodapé)

---

## Como Estilizar o Logotipo com CSS?

Para ajustar o tamanho e posicionamento do logotipo, utilize CSS:

```css
.navbarImg img {
  width: 100%;
  margin: 0 auto;
}
```

E aplique no HTML:

```html
<img src="logo.png" alt="Meu Logotipo" class="logo" />
```

---

## Como Alterar o Logotipo com JavaScript?

Se quiser trocar o logotipo dinamicamente:

```javascript
document.querySelector(".logo").src = "novo-logo.png";
```

---

## Como Testar se o Logotipo Está Correto?

- Verifique no navegador se a imagem está carregando corretamente.
- Use a ferramenta **Inspecionar Elemento (F12)** para ajustar o CSS.
- Teste a responsividade com o modo mobile.

---

## Conclusão

O logotipo é uma peça fundamental da identidade visual do site. Ele deve ser bem posicionado, otimizado para carregar rápido e responsivo para diferentes telas.

---

### 📌 Recursos Adicionais

- [Conversor de PNG para SVG](https://www.pngtosvg.com/)
- [Ferramenta para Otimizar Imagens](https://tinypng.com/)
- [Guia de Design para Logotipos](https://99designs.com/blog/tips/logo-design-tips/)
