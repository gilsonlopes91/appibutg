# Calculadora IBUTG (PWA) — como publicar no GitHub Pages

Arquivos desta pasta: `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`.

## Publicar
1. Crie um repositório **público** no GitHub (ex.: `calculadora-ibutg`).
2. Envie **o conteúdo desta pasta** (não a pasta `pwa` em si) para a raiz do repositório.
3. Em *Settings → Pages*, escolha *Deploy from a branch* → `main` → `/ (root)`.
4. Em poucos minutos o site abre em `https://SEU-USUARIO.github.io/calculadora-ibutg/`.

## Domínio próprio (opcional)
1. Em *Settings → Pages → Custom domain*, informe o subdomínio, por exemplo `ibutg.seudominio.com.br`.
2. No painel de DNS do domínio, crie um registro **CNAME**: `ibutg` → `SEU-USUARIO.github.io`.
3. Quando o certificado for emitido, marque *Enforce HTTPS*.

## Instalar como app
- **Celular (Chrome/Android):** menu ⋮ → *Instalar app*. **iPhone (Safari):** Compartilhar → *Adicionar à Tela de Início*.
- **Computador (Chrome/Edge):** ícone de instalar na barra de endereço.
- Depois do primeiro acesso, funciona offline.

## Ao alterar a página
Aumente o número em `const VERSION = 'ibutg-vN'` no arquivo `sw.js`, para que os aparelhos recebam a versão nova.
