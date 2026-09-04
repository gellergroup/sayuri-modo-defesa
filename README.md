# Entrega — Página de vendas "Modo Defesa: Reconexão com a Energia Feminina" (v1)

**Cliente:** Sayuri de Sousa (via Geller Group) · **Data:** 2026-09-03 · **Status:** v1 aguardando validação de paleta

## Arquivos
- `index.html` — página completa (CSS + JS inline, sem dependência além do Google Fonts)
- `assets/` — vazio por enquanto. Esperado: `sayuri-hero.webp`, `sayuri-sobre.webp`, `og-modo-defesa.jpg`, logo
- Cópia para deploy: `EQUIPE GELLER/arquivos-para-deploy/sayuri-modo-defesa/index.html`
- Repositório: `gellergroup/sayuri-modo-defesa` (GitHub Pages para preview)

## Paleta proposta (para validação)
| Token | Hex | Uso |
|---|---|---|
| Roxo profundo (âncora) | `#4A1A6B` | marca, ícones, links, eyebrows |
| Roxo escuro | `#2E0F45` | seções escuras (Modo Defesa, final), cards de declaração |
| Roxo médio | `#6A3A99` | labels, detalhes |
| Tinta de texto | `#24102F` / `#3D2F4A` / `#6B5D78` | títulos / corpo / secundário |
| Lilás suave | `#E9DDF2` / `#F6F1FA` | tints, seções alternadas |
| Fundo | `#FDFBFE` | base da página |
| Dourado (CTA) | `#E0BC5E` → `#C9A24A` → `#A98431` | botões, selo, números das etapas, detalhes |

Tipografia: **Cormorant Garamond** (títulos, itálicos de acento, assinatura — ecoa o serif da logo) + **Manrope** (texto e labels).

> O roxo foi estimado a partir da imagem da logo. Ao receber o arquivo PNG/SVG, conferir o hex exato e ajustar `--violet` no `:root`.

## O que está pronto
- Estrutura completa no padrão Geller (modelo Aline): hero com headline + foto + CTA, VSL, dor, Modo Defesa (seção escura), por que nada resolveu (2 linguagens), método em 4 etapas, conteúdo + 4 bônus, sobre, depoimentos, faixa rolante, oferta com price-card, garantia com selo, FAQ accordion, CTA final, rodapé com disclaimer
- Copy do copywriter mantida na íntegra (só espaçamento "Não.O" corrigido)
- Botão fixo no mobile, reveal ao rolar, hover-lift nos cards, `prefers-reduced-motion` respeitado
- Responsivo (breakpoints 980 / 900 / 620px)
- Todos os CTAs com `data-checkout`: basta preencher `CHECKOUT_URL` no script do final da página
- Sem emojis (o 🌿 da copy virou ícone de folha em SVG), sem foto de banco de imagem

## Pendências (visíveis na página como placeholders)
1. **Foto da Sayuri** — `assets/sayuri-hero.webp` (4:5, fundo neutro ou recortada) e `assets/sayuri-sobre.webp`. Enquanto não existem, aparece um bloco roxo com a mandala
2. **Logo** em PNG/SVG — hoje o header usa uma mandala desenhada em SVG inspirada na logo; trocar pela oficial e confirmar o hex do roxo
3. **VSL** — colar o embed dentro de `<div class="vsl">` (id `vsl`), substituindo o bloco `.vsl-inner`
4. **Link de checkout** — `CHECKOUT_URL` no script (cartão/Zelle)
5. **Depoimentos reais** — 3 cards placeholder em `#depoimentos` (priorizar sono, energia, inchaço, leitura do corpo)
6. **"X minutos"** (Bônus 3) e **"X meses"** (FAQ "Por quanto tempo tenho acesso?")
7. **Descrição do Bônus 4** (Caderno da Reconexão) — não veio na copy
8. **Bônus 1, 2 e 4** serão produzidos pela Vitória; áudio do Bônus 3 editado pela equipe (notas internas, não estão na página)
9. **GTM / Pixel** — comentários marcados no `<head>` e logo após `<body>`
10. **OG image** — `assets/og-modo-defesa.jpg` (1200×630)
11. **Página de obrigado** — derivar desta após validação da paleta

## Checklist anti-IA (v3.2 web-designer)
- [x] Zero emojis na página
- [x] Nenhuma foto genérica de banco de imagem
- [x] Layout não parece template Canva/Wix (hierarquia serif/sans, kickers, cards com borda e profundidade, seções escuras com motivo da marca)
- [x] Cores e fontes derivadas da logo (roxo) — aguardando confirmação do hex
- [x] Responsivo (mobile + desktop) — testar em 375px e 768px após inserir as fotos
- [x] Acentuação correta em todo texto

## Próximos passos
1. Priscila valida paleta e estrutura
2. Receber foto, logo, VSL, checkout e depoimentos → substituir placeholders
3. Definir hospedagem/editor real e publicar
4. Criar página de obrigado a partir desta base

✓ Humanizer aplicado · copy preservada · 10 padrões anti-cara-de-IA verificados
