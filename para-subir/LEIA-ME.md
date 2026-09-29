# Zips prontos para subir no cPanel da Sayuri

Gerados a partir de `../outputs/produto-01-modo-defesa/` e `../outputs/produto-02-equilibrio-vital/`.
Se alguma página for editada lá, **estes zips ficam velhos** e precisam ser gerados de novo.

| Zip | Produto | Versão | Extrair em |
|---|---|---|---|
| `sayuri-P01-modo-defesa-eua.zip` | Modo Defesa | EUA · US$ 37 | pasta da versão EUA do produto 01 |
| `sayuri-P01-modo-defesa-br.zip` | Modo Defesa | Brasil · R$ 97 | pasta da versão Brasil do produto 01 |
| `sayuri-P02-equilibrio-vital-eua.zip` | Equilíbrio Vital | EUA · US$ 99 | pasta da versão EUA do produto 02 |
| `sayuri-P02-equilibrio-vital-br.zip` | Equilíbrio Vital | Brasil · R$ 347 | pasta da versão Brasil do produto 02 |

Cada zip é autossuficiente: leva as próprias imagens em `assets/`. Por isso funciona em
qualquer endereço — é só extrair o **conteúdo** dentro da pasta de destino, sem deixar
uma pasta extra no caminho.

## Estrutura em discussão no servidor (2026-09-22)

A Priscila criou `modo-defesa-eua/` e `modo-defesa-br/` em `public_html/`. Se essa for a
estrutura final, o endereço antigo `seedofhealth.online/modo-defesa/` (que está no ar e pode
estar em anúncio) precisa de um redirecionamento, senão quebra. Decisão ainda em aberto.

## Material antigo

A pasta espelho antiga e os zips da estrutura anterior continuam em
`EQUIPE GELLER/arquivos-para-deploy/` (`sayuri-modo-defesa/`, `sayuri-modo-defesa.zip` e
`sayuri-modo-defesa-ate-2026-09-04.zip`). São histórico, não usar para subir.

> Zips movidos para cá em 2026-09-22, a pedido da Priscila. A partir de agora, o que se
> sobe no cPanel da Sayuri sai desta pasta.
