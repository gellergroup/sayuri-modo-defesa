# PRODUTO 01 — Modo Defesa: Reconexão com a Energia Feminina

Duas versões, cada uma numa pasta, **cada uma completa e independente**.

```
produto-01-modo-defesa/
├── eua/   ← versão Estados Unidos, US$ 37
│   ├── index.html            página de vendas
│   ├── obrigado/index.html   página de obrigado
│   └── assets/               imagens desta versão
└── br/    ← versão Brasil, R$ 97
    ├── index.html
    ├── obrigado/index.html
    └── assets/
```

As duas têm o mesmo texto. Muda preço, moeda e, no Brasil, o título da aba leva `[BR]`
para você não confundir durante a conferência.

## Onde publicar cada uma

| Pasta | Extrair o zip em |
|---|---|
| `eua/` | `public_html/modo-defesa/` |
| `br/` | `public_html/modo-defesa/br/` |

Cada pasta carrega o próprio `assets/`, então funciona em qualquer endereço — é só
extrair no lugar certo. Nenhum caminho precisa ser reescrito se o produto mudar de lugar.

**Cuidado:** extraia o **conteúdo** da pasta no destino, não a pasta `eua` inteira.
Se subir a pasta junto, o endereço vira `.../eua/` e o link muda.

## `assets/`

Cada versão tem sua cópia de: sayuri-hero.webp e sayuri-sobre.webp, as logos e as 3 avaliações do Google
(`depoimento-*.webp`). Sim, as imagens se repetem entre as pastas — é isso que deixa cada
uma independente e publicável sozinha. São poucos KB.

## Pendências

`og-modo-defesa.jpg` (imagem de compartilhamento), embed da VSL, link de checkout e GTM/Pixel.

> Fonte de verdade das páginas. `EQUIPE GELLER/arquivos-para-deploy/` é só cópia para upload.
> Estrutura separada por produto e por versão em 2026-09-22.
