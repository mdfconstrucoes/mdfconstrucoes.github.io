# Site MDF Construções

Site institucional da MDF Construções e Segurança do Trabalho Ltda.
Publicado em https://mdfconstrucoes.github.io

## Estrutura
- `index.html` página única (serviços, como trabalhamos, região, empresa, FAQ, contato)
- `assets/css/site.css` e `assets/js/main.js` minificados
- `assets/fonts/` fontes hospedadas no próprio site (Archivo, Barlow, IBM Plex Mono)
- `assets/img/` logo, ícones e imagem de compartilhamento (og.png)
- `404.html`, `robots.txt`, `sitemap.xml`, `site.webmanifest`, `.well-known/security.txt`

## Segurança e privacidade
- Content Security Policy: só carrega arquivos do próprio site, sem scripts de terceiros
- Sem cookies, sem rastreadores, sem formulário enviando dados para servidor (o formulário só monta a mensagem e abre o WhatsApp)
- Links externos com `noopener noreferrer`
- HTTPS obrigatório: ative "Enforce HTTPS" em Settings > Pages

## Contato do formulário
WhatsApp +55 35 99220-9440. Para trocar o número, edite `assets/js/main.js` (procure 5535992209440) e os links `wa.me` no `index.html`.

## Domínio próprio (quando comprar mdfconstrucoes.io)
1. Crie um arquivo `CNAME` na raiz com o conteúdo `mdfconstrucoes.io`
2. No painel do registrador, crie registros A apontando para 185.199.108.153, 185.199.109.153, 185.199.110.153 e 185.199.111.153, e um CNAME `www` para `mdfconstrucoes.github.io`
3. Em Settings > Pages, informe o domínio e marque "Enforce HTTPS"
4. Troque `https://mdfconstrucoes.github.io/` por `https://mdfconstrucoes.io/` no `index.html`, `sitemap.xml`, `robots.txt` e `.well-known/security.txt`
