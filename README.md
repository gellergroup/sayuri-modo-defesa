# Entrega — Página de vendas "Modo Defesa: Reconexão com a Energia Feminina" (v1)

**Cliente:** Sayuri de Sousa (via Geller Group) · **Data:** 2026-09-03 · **Status:** v1 aguardando validação de paleta

## Arquivos
- `index.html` — página de vendas completa (CSS + JS inline, sem dependência além do Google Fonts)
- `equilibrio-vital/index.html` — página de vendas do produto 02 (Método Equilíbrio Vital®), **diagramação nova** e **sub-paleta verde** (jade `#3E9C70`, menta `#7FCBA0`, jade escuro `#2A7352`, seções escuras verde-floresta `#0F2A20→#1F5A43`, fundos branco-menta; roxo da marca só em logo/rótulos/itálicos). Elementos: barra de progresso de leitura, cabeçalho fixo com CTA após o hero, VSL dentro do hero escuro, lista de tentativas com marcadores, painel "o nome / o caminho", cadeia dos sintomas, método em linha do tempo, pilares de conteúdo, presentes em lista editorial, sobre com foto sangrada, carrossel de depoimentos (scroll-snap), oferta em caixa dois tons, garantia em "certificado", FAQ em linhas. Pendências próprias: fotos, VSL, preços US$ X / X vezes, garantia X dias, "Acesso por X", `CHECKOUT_URL`, depoimentos
- `equilibrio-vital/obrigado/index.html` — página de obrigado do produto 02 (sub-paleta verde). Confirmação escura com card do pedido + botão "Acessar o programa", seção de pergunta com card do formulário de interesse. `noindex`. Pendências: `MEMBER_URL`, `FORM_URL`, "Acesso por X". Número do pedido via `?pedido=`. "[sobrenome]" preenchido com "de Sousa"
- `obrigado/index.html` — página de obrigado + upsell (Método Equilíbrio Vital), mesma paleta. `noindex`. Pendências próprias: VSL do upsell, "X minutos", preços (US$ XXX / 12x XX,XX), `UPSELL_URL` e `MEMBER_URL` no script, e-mail/WhatsApp de suporte, "Acesso por X". Número do pedido é preenchido automaticamente se a URL vier com `?pedido=` (ou `?order=`). Nome do produto de entrada unificado em 2026-09-11: "Modo Defesa: Reconexão com a Energia Feminina"
- `assets/` — fotos já encaixadas (2026-09-03, escolhidas entre as 13 enviadas em `../../assets/fotos/`): `sayuri-hero.webp` (jaleco branco no consultório → hero do Reset), `sayuri-sobre.webp` (sorriso, mão no queixo → "Quem conduz" do Reset), `sayuri-ev-sobre.webp` (fitoterapia, potes de ervas → "Prazer, sou a Sayuri" do Equilíbrio Vital), `sayuri-ev-hero.webp` (olhar, fundo escuro → hero do Equilíbrio Vital, ao lado da headline), `sayuri-ev-oferta.webp` (blazer verde-musgo → círculo no topo da caixa de oferta do Equilíbrio Vital). Logo oficial recebida em 2026-09-04 (`assets/fotos/3.png`) e aplicada: `logo-sayuri.png` (lockup), `logo-mandala.png` (só a mandala, header + marcas d'água) e versões brancas. Ainda faltam: `og-modo-defesa.jpg`, `og-equilibrio-vital.jpg`
- Cópia para deploy: `EQUIPE GELLER/arquivos-para-deploy/sayuri-modo-defesa/index.html`
- Repositório: `gellergroup/sayuri-modo-defesa` (só histórico de código — sem GitHub Pages, por decisão da Priscila)

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

> Roxo confirmado a partir do arquivo oficial da logo: `--violet: #480070` (aplicado nas 4 páginas em 2026-09-04).

## Versão Brasil (2026-09-11)
- `br/` espelha as 4 páginas da raiz (mesmos assets em `../assets/`, caminhos ajustados). Diferença: preço e moeda. Títulos das abas com prefixo `[BR]` pra distinguir na validação
- EUA (raiz): P1 US$ 37 (era "US$ 47 (ou R$ 297)"; o "ou R$ 297" saiu), P2 US$ 100. Brasil (`/br/`): P1 R$ 97, P2 R$ 347; upsell da obrigado BR em R$ (valores ainda XXX)
- Placeholders novos: "De R$ X" (P1 BR, P2 BR), "De US$ X" (P2 EUA), "X vezes" (P2), valores simbólicos dos bônus (não recebidos)
- Vercel: mesmo projeto, `/br/...`

## Ajustes 2026-09-11 (pedido da Priscila)
- Produto 01 renomeado na página de obrigado: "Modo Defesa: Reconexão com a Energia Feminina" (5 ocorrências)
- Acesso por 1 ano: FAQ do Reset, FAQ do EV, rodapés das duas páginas de obrigado
- Bônus do produto 01: 1 Caderno de Reconexão Modo Defesa (com descrição) · 2 Guia Alimentar Modo Defesa® (só título) · 3 Meditação Guiada para Reduzir o Estresse (12 minutos) · 4 Checklist 4 vazamentos (só título)
- Bônus do EV (mesmo dia, 2ª leva): 6 bônus novos nos cards da vendas EV (título + subtítulo, rótulo "Bônus N"), e na lista da oferta. Bônus 6 "Pergunte à Sayuri" só título. Upsell da obrigado do Reset revertido pra lista original de 5 (fora do pedido). As frases com "5" (presentes/bônus) ficaram como estavam — copy, aguardando autorização pra virar 6
- Vercel `geller-sayuri-modo-defesa` redeployado com tudo isso (11/09)
- **Publicação:** repo atualizado; os 4 arquivos precisam ser reenviados ao cPanel (`seedofhealth.online/modo-defesa/`)

## Passada de UX (2026-09-03, após revisão da Priscila no desktop)
- Corrigida especificidade de CSS que encolhia destaques: pergunta grande em itálico (EV), assinatura "Sayuri de Sousa" (Reset, sobre e final), frase dos "luxos" na seção Modo Defesa (Reset), assinatura no sobre (EV)
- Presentes (EV): saiu o layout coluna vazia + lista; agora título centralizado e 6 cards em 2 colunas (5 presentes + card verde de CTA)
- Tentativas (EV): pílula do ciclo subiu pra coluna do título, que fica fixa ao rolar
- Depoimentos (EV): setas anterior/próximo no carrossel (desktop não consegue arrastar com mouse)
- Obrigado EV: coluna do título centralizada verticalmente em relação ao card do formulário; mandala reposicionada
- Removidas duas linhas que não estavam na copy (subtítulo do FAQ e item da lista da oferta com travessão)
- Equilíbrio Vital: Sayuri no hero (retrato ao lado da headline) e no topo da caixa de oferta (círculo)
- Obrigado EV: seção da pergunta em coluna única (título → texto → destaque → card do formulário)
- **Regra Geller aplicada:** no mobile, a foto vem antes da headline nos heros das duas páginas de vendas (`order: -1`, recorte ~1:1)

## O que está pronto
- Estrutura completa no padrão Geller (modelo Aline): hero com headline + foto + CTA, VSL, dor, Modo Defesa (seção escura), por que nada resolveu (2 linguagens), método em 4 etapas, conteúdo + 4 bônus, sobre, depoimentos, faixa rolante, oferta com price-card, garantia com selo, FAQ accordion, CTA final, rodapé com disclaimer
- Copy do copywriter mantida na íntegra (só espaçamento "Não.O" corrigido)
- Botão fixo no mobile, reveal ao rolar, hover-lift nos cards, `prefers-reduced-motion` respeitado
- Responsivo (breakpoints 980 / 900 / 620px)
- Todos os CTAs com `data-checkout`: basta preencher `CHECKOUT_URL` no script do final da página
- Sem emojis (o 🌿 da copy virou ícone de folha em SVG), sem foto de banco de imagem

## Pendências (visíveis na página como placeholders)
1. **Foto da Sayuri** — `assets/sayuri-hero.webp` (4:5, fundo neutro ou recortada) e `assets/sayuri-sobre.webp`. Enquanto não existem, aparece um bloco roxo com a mandala
2. ~~**Logo** em PNG/SVG~~ — feito em 2026-09-04: header e marcas d'água usam a mandala real (`assets/logo-mandala.png`), hex do roxo confirmado
3. **VSL** — colar o embed dentro de `<div class="vsl">` (id `vsl`), substituindo o bloco `.vsl-inner`
4. **Link de checkout** — `CHECKOUT_URL` no script (cartão/Zelle)
5. **Depoimentos reais** — 3 cards placeholder em `#depoimentos` (priorizar sono, energia, inchaço, leitura do corpo)
6. ~~"X minutos" e "X meses"~~ — resolvido 2026-09-11 (12 minutos / 1 ano)
7. ~~Descrição do Bônus 4~~ — lista de bônus substituída em 2026-09-11 (bônus 2 e 4 só com título, por decisão)
8. Bônus produzidos pela Vitória / áudio pela equipe (notas internas, não estão na página)
9. **GTM / Pixel** — comentários marcados no `<head>` e logo após `<body>`
10. **OG image** — `assets/og-modo-defesa.jpg` (1200×630)
11. **Página de obrigado** — derivar desta após validação da paleta

## Checklist anti-IA (v3.2 web-designer)
- [x] Zero emojis na página
- [x] Nenhuma foto genérica de banco de imagem
- [x] Layout não parece template Canva/Wix (hierarquia serif/sans, kickers, cards com borda e profundidade, seções escuras com motivo da marca)
- [x] Cores e fontes derivadas da logo (roxo) — hex confirmado pelo arquivo oficial (#480070)
- [x] Responsivo (mobile + desktop) — testar em 375px e 768px após inserir as fotos
- [x] Acentuação correta em todo texto

## Próximos passos
1. Priscila valida paleta e estrutura
2. Receber foto, logo, VSL, checkout e depoimentos → substituir placeholders
3. ~~Definir hospedagem/editor real e publicar~~ — no ar em `seedofhealth.online/modo-defesa/` (2026-09-04, cPanel, pasta `public_html/modo-defesa/`)
4. Criar página de obrigado a partir desta base

✓ Humanizer aplicado · copy preservada · 10 padrões anti-cara-de-IA verificados
