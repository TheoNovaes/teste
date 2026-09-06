# [NOME DA LOJA] — Site de Loja de Tênis (10 páginas)

Projeto estático em HTML5 + CSS3 puro, sem frameworks e sem JavaScript de
máscara (validação 100% nativa do HTML5). Todos os textos entre colchetes
(`[assim]`) são placeholders — substitua pelos dados reais da loja.

## Estrutura de arquivos

```
loja-tenis/
├── index.html                  → Página inicial
├── sobre.html                  → Institucional (contém áudio)
├── produtos.html                → Catálogo geral (tabela + cards)
├── masculino.html                → Categoria masculina
├── feminino.html                 → Categoria feminina
├── produto-detalhe.html          → Ficha de produto (contém vídeo + tabela de numeração)
├── guia-de-numeracao.html        → Tabela de conversão BR/US/EU
├── trocas-e-devolucoes.html      → Política de trocas
├── orcamento.html                 → Formulário de orçamento (compra em quantidade)
├── contato.html                   → Formulário de contato
├── css/
│   └── style.css                → CSS único e principal do site
└── assets/
    ├── img/                       → Fotos dos produtos (adicionar)
    ├── audio/                     → institucional.mp3 (adicionar)
    └── video/                     → produto-demonstracao.mp4 (adicionar)
```

## O que já está pronto

- Estrutura semântica completa (`header`, `nav`, `main`, `section`, `article`, `footer`) em todas as páginas
- Navegação idêntica e funcional entre as 10 páginas, com `aria-current="page"` marcando a página ativa
- `<audio>` em `sobre.html` e `<video>` em `produto-detalhe.html`
- Dois formulários com validação nativa do HTML5:
  - `type="email"`, `type="tel"` com `pattern`, `type="number"`, `type="date"`
  - `required`, `minlength`, `maxlength`, `min`, `max`
  - Nenhuma biblioteca de máscara — tudo via atributos HTML5
- CSS único (`style.css`) organizado por seções, com variáveis em `:root`
- Componentes reutilizáveis (`.card-produto`, `.btn`, tabelas, formulários) usados de forma consistente
- Layout responsivo (media queries para tablet e celular)

## O que você precisa preencher/ajustar

1. **Identidade visual**: troque as variáveis de cor e fonte em `css/style.css` (`:root`) pela marca real
2. **Textos entre colchetes**: nome da loja, textos institucionais, descrições de produtos, preços
3. **Imagens reais**: substitua os blocos `.imagem-placeholder` / `.imagem-produto` por `<img>` com `src` e `alt` reais
4. **Arquivos de mídia**: adicione `institucional.mp3` em `assets/audio/` e `produto-demonstracao.mp4` em `assets/video/`
5. **`feminino.html`**: foi gerado a partir de `masculino.html` — confira se os produtos de exemplo fazem sentido

## Antes de entregar

1. Valide **cada uma das 10 páginas** em https://validator.w3.org/#validate_by_upload
2. Corrija qualquer erro/warning (atributos `alt` faltando, tags não fechadas, `id` duplicado etc.)
3. Teste os formulários preenchendo campos errados (e-mail sem @, telefone fora do padrão) para confirmar que o navegador bloqueia o envio
4. Suba o projeto para um repositório no GitHub com commits organizados (não um único commit)
5. Ative o GitHub Pages para testar a responsividade em um link público
