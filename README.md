# Koncept Experience — Landing page

Landing page da academia Koncept Experience (Setor Industrial do Gama, Brasília - DF).

Site estático em HTML, CSS e JavaScript puro, sem etapa de build.

## Como colocar ou trocar as fotos (sem mexer em código)

Cada espaço "FOTO REAL AQUI" do site procura uma foto com um nome fixo dentro da pasta `assets/fotos`.

| Nome do arquivo | Onde aparece | Tamanho sugerido |
| --- | --- | --- |
| `ambiente.jpg` | Seção "Sobre a Koncept" | 1200 × 900 |
| `musculacao.jpg` | Galeria, quadro grande | 1200 × 1200 |
| `cardio.jpg` | Galeria, quadro pequeno | 800 × 600 |
| `sala-aulas.jpg` | Galeria, quadro pequeno | 800 × 600 |
| `fachada.jpg` | Galeria, quadro largo | 1200 × 600 |

**Passo a passo pelo site do GitHub:**

1. No computador, renomeie a foto com o nome da tabela (minúsculas, sem acento e sem espaço).
2. Abra a pasta [`assets/fotos`](assets/fotos) neste repositório.
3. Clique em **Add file → Upload files** e arraste a foto.
4. Clique em **Commit changes**.
5. Em cerca de 1 minuto a Vercel publica o site com a foto nova.

Para trocar uma foto, envie outra com o mesmo nome. Formatos aceitos: `.jpg`, `.jpeg`, `.png` e `.webp`. Prefira arquivos com menos de 500 KB (dá para reduzir de graça em [squoosh.app](https://squoosh.app)).

## Visualizar localmente

```
python -m http.server 5500
```

Depois abra http://localhost:5500

## Publicar na Vercel

Importe este repositório na Vercel com o framework **Other** (sem comando de build). Cada push na branch `main` publica uma nova versão.

## Antes de publicar

- O site está em https://koncept-three.vercel.app. Se trocar de domínio, atualize o endereço em `index.html`, `robots.txt`, `sitemap.xml` e `llms.txt`.
- Envie as fotos reais para `assets/fotos` (veja "Como colocar ou trocar as fotos").
- Ao mudar as perguntas frequentes, atualize também o bloco JSON-LD `FAQPage` no `<head>`.
- O cronograma de aulas fica na seção `#aulas`; o status automático usa `AVISO_ANTES_MIN` e `DURACAO_AULA_MIN` no script.
