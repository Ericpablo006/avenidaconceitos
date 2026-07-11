# Avenida Conceito — Link na Bio

Página "link na bio" da loja Avenida Conceito (Ituberá, BA). Site estático, sem build, sem dependências — HTML, CSS e JS puros em um único arquivo.

## Estrutura

```
avenida-conceito/
├── index.html      # página completa (HTML + CSS + JS inline)
├── vercel.json      # config mínima da Vercel
├── .gitignore
└── README.md
```

## Publicar no GitHub

```bash
cd avenida-conceito
git init
git add .
git commit -m "Primeira versão do link na bio"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/avenida-conceito.git
git push -u origin main
```

## Publicar na Vercel

**Opção 1 — pelo site**
1. Acesse https://vercel.com/new
2. Importe o repositório do GitHub
3. Framework Preset: **Other** (site estático, não precisa de build)
4. Build Command: deixe vazio
5. Output Directory: deixe vazio (raiz do projeto)
6. Deploy

**Opção 2 — pela CLI**
```bash
npm i -g vercel
cd avenida-conceito
vercel
```

## Editar os links / textos

Tudo fica no objeto `CONFIG` dentro do `<script>` no final do `index.html` — nome, avatar, e a lista `links` (WhatsApp, Instagram, TikTok etc). Basta editar ali, sem precisar mexer no resto do código.
