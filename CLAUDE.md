# CLAUDE.md — ATELIERDOBANHO

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** ATELIERDOBANHO
**Nicho:** Moda e Beleza
**Keywords:** Bem vindo ao Atelie do Banho o seu destino para produtos de
**Paleta de cores:** forest | **Fonte:** inter

Bem-vindo ao Ateliê do Banho, o seu destino para produtos de cosméticos de alta qualidade! Aqui, oferecemos uma ampla seleção de itens cuidadosamente selecionados para ajudá-lo a cuidar da sua pele, cabelos e corpo. Nossa loja online apresenta uma variedade de cosméticos, desde cremes hidratantes até shampoos e condicionadores de alta qualidade, passando por sabonetes, óleos essenciais e outros produtos para o cuidado pessoal. Todos os nossos produtos são produzidos com ingredientes naturais e de origem sustentável, garantindo que você está cuidando de si mesmo enquanto cuida do planeta. No Ateliê do Banho, estamos comprometidos em fornecer a você a melhor experiência de compra online possível. Navegue em nosso site para encontrar o produto perfeito para você ou presenteie alguém especial. Com envio para todo o Brasil e uma equipe de atendimento ao cliente disponível para ajudá-lo em todas as etapas, estamos aqui para ajudá-lo a cuidar de si mesmo de uma forma consciente e saudável. Experimente o poder dos cosméticos naturais e de qualidade com o Ateliê do Banho – a sua loja online de beleza e bem-estar!



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-E |
| Features | Features-D |
| About Section | About-B |
| Posts | Posts-E |
| Footer | Footer-B |
| Página Sobre | Sobre-H |
| Página Contato | Contato-B |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
