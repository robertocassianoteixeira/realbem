# Realbem Clube — Protótipo Navegável

Protótipo clicável do app **Realbem Clube** (clube de benefícios), construído a partir das telas de UI originais. Simula o fluxo de um usuário visitante fazendo login e navegando pelas áreas do app.

🔗 **Acesse:** `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`
*(atualize este link depois de ativar o GitHub Pages)*

## Como usar

Abra o link em qualquer navegador (celular ou desktop). Toque/clique nas áreas destacadas da tela — menu, botões, cartões — para navegar entre as telas, igual a um protótipo do Figma.

Controles disponíveis abaixo do aparelho:
- **← Voltar** — retorna à tela anterior
- **🏠 Início** — volta para a tela de abertura (splash)
- **Seletor de telas** — pula direto para qualquer tela do fluxo

## Fluxo mapeado

```
Splash
  └─ Home (deslogado)
       ├─ Menu (deslogado)
       │    └─ Login → Home (logado)
       └─ Login (aviso de acesso) → Home (logado)

Home (logado)
  ├─ Menu (logado / Freemium)
  │    ├─ Ver benefícios → Benefícios / Bem Plus
  │    └─ Finalizar sessão → Home (deslogado)
  ├─ Conquistas
  ├─ Benefícios / Bem Plus
  └─ Ofertas

Barra inferior (Home / Conquistas / Benefícios / Ofertas)
disponível em todas as telas logadas
```

Telas ainda não desenhadas no material original (Planos, Perfil, Pagamentos, Central de Ajuda) mostram um aviso de "em construção" em vez de travar a navegação.

## Detalhes técnicos

- Arquivo único (`index.html`), sem dependências externas — todas as imagens das telas estão embutidas em base64.
- Sem backend, sem build step: qualquer hospedagem de arquivo estático serve (GitHub Pages, Netlify, Vercel).
- Peso do arquivo: ~2,3 MB (por causa das imagens embutidas).

## Origem do material

Telas extraídas do arquivo de UI `UI_Realbem_Clube-140426.zip` (exportação do Figma). Este protótipo é um recorte não oficial para fins de teste de navegação — não reflete necessariamente a especificação final do produto.
