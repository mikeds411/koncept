# Koncept Experience — Landing page

Landing page da academia Koncept Experience (Setor Industrial do Gama, Brasília - DF).

Site estático em HTML, CSS e JavaScript puro, sem etapa de build.

## Visualizar localmente

```
python -m http.server 5500
```

Depois abra http://localhost:5500

## Publicar na Vercel

Importe este repositório na Vercel com o framework **Other** (sem comando de build). Cada push na branch `main` publica uma nova versão.

## Antes de publicar

- Troque `https://SEU-DOMINIO.com.br` pelo endereço real em `index.html`, `robots.txt`, `sitemap.xml` e `llms.txt`.
- Substitua os espaços marcados como **FOTO REAL AQUI** (procure por `TROCAR:` no `index.html`).
- Ao mudar as perguntas frequentes, atualize também o bloco JSON-LD `FAQPage` no `<head>`.
- O cronograma de aulas fica na seção `#aulas`; o status automático usa `AVISO_ANTES_MIN` e `DURACAO_AULA_MIN` no script.
