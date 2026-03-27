# Jivago Menezes — Portfolio

Site de portfolio pessoal. HTML/CSS/JS estático, arquivo único, zero dependências externas além do Google Fonts.

## Stack
- `index.html` — o site inteiro
- Tipografia: Newsreader (display) + Manrope (body) + Space Grotesk (labels)
- Cores: burnt orange `#e8864a` como acento principal, teal `#3da89b` para tech tags
- Dark mode, mobile-responsive, sem frameworks

## Publicar no GitHub Pages

```bash
# 1. Cria o repo com este nome exacto
#    github.com/new → nome: jivagomenezes.github.io

# 2. Clona e adiciona os ficheiros
git clone https://github.com/jivagomenezes/jivagomenezes.github.io
cd jivagomenezes.github.io
cp /caminho/para/index.html .

# 3. Publica
git add .
git commit -m "initial portfolio"
git push origin main

# 4. Activa Pages
# GitHub → Settings → Pages → Source: main / root
# URL final: https://jivagomenezes.github.io
```

## Domínio próprio (opcional)

```bash
# Cria ficheiro CNAME na raiz do repo
echo "jivago.dev" > CNAME
git add CNAME && git commit -m "add custom domain" && git push
```

Depois no registador de domínio, cria 4 registos A:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

E um CNAME: `www` → `jivagomenezes.github.io`

## OG Image

Cria um ficheiro `og-image.png` (1200×630px) na raiz do repo.
Pode ser um screenshot do hero do site. As meta tags já apontam para ele.

## Estrutura de ficheiros recomendada

```
jivagomenezes.github.io/
├── index.html        ← o site
├── CNAME             ← só se tiveres domínio próprio
├── og-image.png      ← imagem para partilha social
└── README.md
```

## Para continuar no Claude Code

```bash
npm install -g @anthropic/claude-code
cd jivagomenezes.github.io
claude
```

Ver CLAUDE.md para contexto completo do projecto.
