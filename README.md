# Favicon: Tudo o que Você Precisa Saber

## O que é um Favicon?

O **favicon** ("favorite icon") é um pequeno ícone associado a um site ou página da web. Ele aparece em várias partes do navegador, como:

- Aba do navegador
- Barra de favoritos
- Histórico de navegação
- Atalhos na tela inicial em dispositivos móveis
- Resultados de pesquisa no Google (em alguns casos)

### Exemplo de favicon exibido na aba do navegador:

![Exemplo de Favicon](https://github.com/DRMEducacao/Template-Ocean/blob/main/check-listBeforeDelivery/image/faviconExample.jpg)

---

## Como Criar um Favicon?

Você pode criar um favicon usando ferramentas gráficas ou geradores online. Ele deve ter um design simples, pois será exibido em tamanhos pequenos.

### Requisitos:

- Formatos comuns: `.ico`, `.png`, `.svg`, `.jpg` (recomendado `.ico` ou `.png` para compatibilidade total)
- Tamanho recomendado: `16x16px`, `32x32px` ou `48x48px` (para diferentes resoluções de tela)
- Fundo transparente (preferível para melhor adaptação a diferentes temas de navegador)

### Ferramentas para criar um favicon:

- [Favicon.io](https://favicon.io/)
- [RealFaviconGenerator](https://realfavicongenerator.net/)
- [Canva](https://www.canva.com/)
- [GIMP](https://www.gimp.org/)
- [Adobe Photoshop](https://www.adobe.com/products/photoshop.html)

Exemplo de favicon no formato `.ico`:
![Exemplo de Favicon](https://euestudo.com.vc/sys/images/icon.png)

---

## Como Adicionar um Favicon ao Seu Site

### Método 1: Na plataforma da DRM

Clique em "Meu Site":
![Meu Site](https://github.com/DRMEducacao/Template-Ocean/blob/main/check-listBeforeDelivery/image/meuSite.png)

Depois em "Página Principal":
![Página principal](https://github.com/DRMEducacao/Template-Ocean/blob/main/check-listBeforeDelivery/image/mainPage.png)

Depois em "Logotipo e ícone":
![Logotipo e ícone](https://github.com/DRMEducacao/Template-Ocean/blob/main/check-listBeforeDelivery/image/faviconExample.png)

Na tela seguinte, faça o upload do logotipo obedecendo as especificações:
![Logotipo e ícone](https://github.com/DRMEducacao/Template-Ocean/blob/main/check-listBeforeDelivery/image/lista.png)

E pronto! Agora basta aguardar a propagação que poderá levar até 4 horas.

### Método 2: Adicionando via HTML

Após criar seu favicon, adicione a seguinte linha dentro da seção `<head>` do seu HTML:

```html
<link rel="icon" type="image/png" href="favicon.png" />
```

Ou para formato `.ico`:

```html
<link rel="icon" type="image/x-icon" href="favicon.ico" />
```

### Método 3: Adicionando via Manifest.json (para PWA)

Se seu site for um Progressive Web App (PWA), você pode adicionar o favicon no `manifest.json`:

```json
{
  "name": "Meu Site",
  "icons": [
    {
      "src": "favicon-192x192.png",
      "type": "image/png",
      "sizes": "192x192"
    },
    {
      "src": "favicon-512x512.png",
      "type": "image/png",
      "sizes": "512x512"
    }
  ]
}
```

### Método 4: Adicionando via `.htaccess`

Se deseja definir um favicon padrão para todo o site sem precisar editá-lo no HTML, adicione a seguinte linha no `.htaccess`:

```apache
AddType image/x-icon .ico
Redirect 301 /favicon.ico https://meusite.com/favicon.ico
```

---

## Testando seu Favicon

Após adicionar o favicon, limpe o cache do navegador e recarregue a página para verificar se ele aparece corretamente. Você também pode testar usando:

- [RealFaviconGenerator](https://realfavicongenerator.net/favicon_checker)
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse/)

---

## Conclusão

O favicon é um pequeno detalhe, mas faz uma grande diferença na identidade visual e na usabilidade do site. Certifique-se de usar um design simples e formatos compatíveis para garantir uma boa experiência para os usuários!

---

### 📌 Recursos Adicionais

- [Documentação MDN sobre Favicons](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/link#favicons)
- [Compatibilidade de Favicons em Diferentes Navegadores](https://caniuse.com/link-icon)
