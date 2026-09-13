# Teste — Página de vendas, 2 dobras (Sayuri de Sousa / Modo Defesa)

**Status:** rascunho de teste. Não publicar, não linkar, não deployar.

## O que é

Página de vendas reduzida a apenas 2 dobras, para validar layout isoladamente:

1. **Hero** — headline, lead, CTA, stats, foto
2. **Oferta / CTA** — argumento de oferta, stack de itens inclusos, price card

## Copy

100% placeholder, gerada só para este teste (autorizado por Priscila em 2026-09-13: "crie uma só pra teste").
**Não é copy final aprovada** — não reaproveitar em página real sem trocar pelo texto oficial.

## Paleta e componentes

Reaproveitados literalmente de `outputs/2026-09-modo-defesa-lp/index.html` (página real, intocada):
roxo profundo `#480070` + dourado `#c9a24a`, Cormorant Garamond + Manrope, mandala SVG, hero com foto
sangrando (regra mobile: foto antes do headline), price card com selo/preço/CTA.

## Assets

Cópias de `outputs/2026-09-modo-defesa-lp/assets/`: `logo-mandala.png`, `sayuri-hero.webp`.
Nenhum arquivo da página real foi alterado.

## Checklist anti-IA (protocolo Geller)

- [x] Zero emoji
- [x] Zero travessão em texto corrido (banner/rodapé ajustados)
- [x] `node --check` no script inline (OK)
- [x] Foto visível no mobile, antes do headline
- [x] CTA sinalizado como placeholder (`CHECKOUT_URL = null`), nenhum link inventado
- [x] Rótulos `[Teste]` / `[Placeholder]` visíveis em todo texto de teste

## Pendências

- Copy final (quando a Priscila decidir usar este layout em produção)
- Checkout real
- Aprovação de layout antes de qualquer publicação
