# Google Tag Manager (GTM): Tudo o que Você Precisa Saber

## O que é o Google Tag Manager (GTM)?

O **Google Tag Manager (GTM)** é uma ferramenta gratuita do Google que permite gerenciar e implementar tags (scripts) em um site sem a necessidade de alterar diretamente o código-fonte. Ele facilita a adição de rastreamentos como Google Analytics, Facebook Pixel, entre outros.

### Benefícios do GTM:

✅ **Facilidade de gerenciamento** – Adicione ou edite tags sem mexer no código do site.  
✅ **Maior desempenho** – Carrega as tags de forma assíncrona, sem afetar a velocidade do site.  
✅ **Maior controle** – Ative/desative tags conforme regras definidas.  
✅ **Melhor integração** – Funciona com Google Analytics, Ads, Facebook Pixel e outras ferramentas.

---

## Como Configurar o Google Tag Manager?

1. **Crie uma conta no GTM**
   - Acesse [Google Tag Manager](https://tagmanager.google.com/)
   - Clique em **Criar Conta** e preencha as informações do site.
2. **Adicione o código ao seu site**

Geralmente, para adicionar a tag do GTM em um site, é necessário ter acesso ao código-fonte da página e conhecimento básico sobre HTML. No entanto, facilitamos esse processo para que a adição da tag (código) ao nosso sistema seja mais ágil sem a necessidade de manipulação do código-fonte da página. Veja a seguir:

Obtenha o código da tag da conta criada:
![GTM Code](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/gtm/image/gtmCode.png)

Vá para "Meu Site":
![Meu Site](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/page-favicon/image/meuSite.png)

Depois para "Administração":
![Administração](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/title-page/image/admin.png)

Depois para "Google Tag Manager":
![Google Tag Manager](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/gtm/image/gtm.png)

Clique em "+" para adicionar uma nova tag:
![Adicionar nova](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/gtm/image/addNew.png)

E adicione ou cole exatamente o mesmo código no campo exibido:
![Colar código GTM](https://github.com/IsaiasSantanaDosSantos/O-QUE-E-FAVICON/blob/main/gtm/image/salve.png)

Pronto!

Apenas para conhecimento, veja como seria caso precisasse adicionar manualmente...

Ao criar sua conta, basta copiar o código da tag

- O GTM fornecerá dois trechos de código.
- O primeiro deve ser colocado no `<head>`:

```html
<!-- Google Tag Manager -->
<script>
  (function (w, d, s, l, i) {
    w[l] = w[l] || [];
    w[l].push({ "gtm.start": new Date().getTime(), event: "gtm.js" });
    var f = d.getElementsByTagName(s)[0],
      j = d.createElement(s),
      dl = l != "dataLayer" ? "&l=" + l : "";
    j.async = true;
    j.src = "https://www.googletagmanager.com/gtm.js?id=" + i + dl;
    f.parentNode.insertBefore(j, f);
  })(window, document, "script", "dataLayer", "GTM-XXXXXX");
</script>
<!-- Fim Google Tag Manager -->
```

- O segundo deve ser adicionado no `<body>`:

```html
<!-- Google Tag Manager (noscript) -->
<noscript
  ><iframe
    src="https://www.googletagmanager.com/ns.html?id=GTM-XXXXXX"
    height="0"
    width="0"
    style="display:none;visibility:hidden"
  ></iframe
></noscript>
<!-- Fim Google Tag Manager (noscript) -->
```

---

## Como Criar e Gerenciar Tags no GTM?

1. **Acesse sua conta no GTM.**
2. **Vá para a aba "Tags" e clique em "Nova".**
3. **Escolha o tipo de tag** (Google Analytics, Facebook Pixel, etc.).
4. **Defina os gatilhos** (quando a tag será ativada, como em cliques ou visualização de página).
5. **Salve e publique** as alterações.

---

## Como Verificar se o GTM Está Funcionando?

1. **Use a extensão "Tag Assistant" do Google** para testar a implementação.
2. **Acesse o modo "Preview" no GTM** para verificar se as tags estão disparando corretamente.
3. **Verifique no Google Analytics** se os eventos estão sendo registrados.

---

## Conclusão

O Google Tag Manager é uma ferramenta essencial para gerenciar tags e rastreamentos sem precisar modificar o código do site constantemente. Ele melhora a organização, otimiza o carregamento e facilita integrações com diversas plataformas.

---

### 📌 Recursos Adicionais

- [Guia Oficial do GTM](https://support.google.com/tagmanager/)
- [Verificador de Tags do Google](https://tagassistant.google.com/)
- [Curso Gratuito de Google Tag Manager](https://analytics.google.com/analytics/academy/)
