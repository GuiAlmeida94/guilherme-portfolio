# Portfólio — Guilherme Oyakawa

Site estático (HTML/CSS/JS puro, sem build). Pronto pra publicar no GitHub Pages, de graça.

## Arquivos
- `index.html` — a página principal (estilo já embutido no arquivo)
- `projects/` — uma página própria para cada projeto (processo completo, achados e impacto), também com estilo embutido
- `robots.txt` e `sitemap.xml` — indexação para o Google
- `CNAME` — configura o domínio próprio no GitHub Pages

## Como publicar (GitHub Pages)

1. Crie um repositório novo no GitHub (ex: `guilherme-portfolio`), público.
2. Suba todos esses arquivos e a pasta `projects/` (mantendo a estrutura) pra raiz do repositório (pelo site do GitHub: "Add file" → "Upload files", ou via `git push`).
3. Vá em **Settings → Pages** do repositório.
4. Em "Build and deployment", escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`. Salve.
5. Em alguns minutos o site estará no ar em `https://SEU-USUARIO.github.io/guilherme-portfolio/`.

## Conectar seu domínio (guilhermeoyakawa.com.br)

O arquivo `CNAME` já está configurado para `www.guilhermeoyakawa.com.br`. Falta apontar o DNS:

1. No painel do seu registrador de domínio, crie um registro **CNAME**:
   - Nome/host: `www`
   - Valor: `SEU-USUARIO.github.io`
2. Para o domínio raiz (`guilhermeoyakawa.com.br` sem `www`) funcionar também, crie registros **A** apontando para os IPs do GitHub Pages:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
3. De volta em **Settings → Pages** no GitHub, digite `www.guilhermeoyakawa.com.br` no campo de domínio customizado e marque **Enforce HTTPS** (pode levar algumas horas para o certificado ser emitido).

## O que ajustar antes de publicar

- O número de WhatsApp no site é o italiano (+39...) que já estava no site antigo — se quiser, troque pelo número atual.
- Não incluí sua foto (não consegui reaproveitar a do Google Sites com segurança). Se quiser adicionar, é só colocar o arquivo de imagem na pasta e referenciar no `index.html`.
- A seção "About" ficou mais enxuta que a versão atual — tirei a parte de peso/objetivo de emagrecimento e a história da sua mãe, que achei mais pessoal demais pra um portfólio profissional. Se quiser reincluir algo, me avise ou edite direto no HTML.
