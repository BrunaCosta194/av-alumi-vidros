# AV Alumi Vidros — Site Institucional

Site estático da AV Alumi Vidros, distribuidora de vidros e alumínio em Jacareí, SP.

## Estrutura

```
av-alumi-vidros/
├── index.html       # Único arquivo do site — todo HTML, CSS e JS embutido
├── assets/
│   ├── logo-av.jpg
│   ├── cebrace.jpg
│   └── parceiro-al.jpg
└── .gitignore
```

## Stack

- HTML/CSS/JS puro, sem framework, sem build tool
- Site de página única (`index.html`, ~1700 linhas)
- Hospedado no **Cloudflare Pages** com deploy automático via GitHub
- Repositório: `https://github.com/BrunaCosta194/av-alumi-vidros`

## Deploy

Qualquer `git push` para a branch `main` dispara deploy automático no Cloudflare Pages (~1 min).

```bash
git add index.html
git commit -m "descrição da mudança"
git push
```

## Responsividade Mobile

Hamburger menu CSS-only (checkbox trick) ativado em `max-width: 640px`.
Ajustes de padding e tamanho de fonte em `max-width: 480px`.
Os `data-chip` são ocultados em mobile (`display: none`) para evitar overflow horizontal.

## Seções do Site

1. **Nav** — logo + links + CTA "Solicitar Orçamento"
2. **Hero** — headline, subtítulo, botões, stats (anos, produtos, atendimentos)
3. **Produtos** — cards de categorias (vidro temperado, box, espelhos, etc.)
4. **Sobre** — história da empresa, diferenciais
5. **CTA** — banner de conversão com botão WhatsApp
6. **Localização** — mapa iframe + endereço + horário
7. **Footer**
