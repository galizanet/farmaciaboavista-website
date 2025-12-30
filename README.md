# Farmácia Boa Vista — Website (landing page)

Site simples e rápido para direcionar clientes ao atendimento **via WhatsApp**.

## ✅ O que este projeto faz

- Landing page estática (HTML/CSS/JS)
- CTA forte para iniciar conversa no WhatsApp: **+55 74 99961-0046**
- Seções: Serviços, Como pedir, Entrega, Contato
- Pronto para publicar no **Cloudflare Pages** conectado ao GitHub

## 📁 Estrutura

- `index.html`
- `styles.css`
- `script.js`
- `assets/logo.svg` (placeholder — troque pela logo oficial)

## 🖼️ Trocar a logo

1. Baixe a logo oficial (ex.: da página do Facebook).
2. Substitua o arquivo: `assets/logo.svg`  
   - Se tiver PNG, use `assets/logo.png` e atualize os caminhos em `index.html`.

> Dica: também atualize `assets/og-image.png` (preview do WhatsApp / redes sociais).
> Se não tiver, remova as tags `og:image` do `index.html`.

## 🚀 Deploy no Cloudflare Pages (recomendado)

### 1) Criar o repositório

Repositório sugerido:
- `https://github.com/galizanet/farmaciaboavista-website`

Commit e push destes arquivos para o branch `main`.

### 2) Conectar no Cloudflare Pages

No Cloudflare Dashboard:
1. **Workers & Pages → Create application → Pages → Connect to Git**
2. Selecione o repo `galizanet/farmaciaboavista-website`
3. Framework preset: **None**
4. Build command: *(vazio)*
5. Output directory: *(vazio / root)*

Deploy.

### 3) Domínio customizado: www.farmaciaboavista.com.br

No seu projeto Pages:
- **Custom domains → Set up a custom domain**
- Adicione: `www.farmaciaboavista.com.br`

Cloudflare vai orientar a configuração de DNS.

#### Recomendação de DNS
- `www` → **CNAME** para `<seu-projeto>.pages.dev`
- Apex (`farmaciaboavista.com.br`) → crie redirect para `www`
  - Pages → **Redirects** (ou Cloudflare Bulk Redirects)

## 🧭 SEO básico (rápido)

- Atualize o `meta description` no `index.html`
- Confirme endereço, horário e links sociais oficiais

## 🔒 Boas práticas
- Não exibir promessas clínicas
- Incluir aviso de prescrição para medicamentos controlados
- Colocar link para Política de Privacidade (se usar forms/cookies futuramente)

---

Feito para publicação rápida e evolução incremental.
