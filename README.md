# Cássio Bragança — Psicologia

Landing page de página única (HTML5 + CSS3 puro, sem frameworks) para o
psicólogo clínico **Cássio Bragança (CRP 06/229036)**, pronta para rodar
estaticamente no GitHub Pages.

## Arquivos

- `index.html` — estrutura semântica da página (header, hero, agendamento, footer e botão de WhatsApp).
- `style.css` — estilos com variáveis CSS (`:root`), design mobile-first e comentários.
- `.github/workflows/deploy.yml` — workflow de deploy automático no GitHub Pages.

## Personalização (passos rápidos)

1. **Agenda do Google:** no `index.html`, dentro da `div.calendar-container`,
   substitua `COLE_AQUI_O_LINK_DE_EMBED_DO_GOOGLE` no atributo `src` do
   `<iframe>` pelo link de *embed* da sua "Página de agendamento de horários"
   do Google Calendar.
2. **WhatsApp:** no link do botão flutuante (`a.whatsapp-float`), troque o
   número `5500000000000` pelo seu número real (formato internacional, ex.:
   `55` + DDD + número) e ajuste a mensagem padrão, se desejar.

## Deploy automático (GitHub Pages via GitHub Actions)

O deploy acontece automaticamente a cada `push` na branch `main`. Para ativar:

- Acesse **Settings** (Configurações) do repositório no GitHub.
- No menu lateral, clique em **Pages**.
- Em **Build and deployment → Source**, selecione **GitHub Actions**.
- Faça um `push` na branch `main` (ou rode o workflow manualmente em **Actions → Deploy to GitHub Pages → Run workflow**).
- Aguarde a conclusão do workflow; o site ficará disponível em
  `https://<seu-usuario>.github.io/<repositorio>`.

> Observação: o deploy inicial usa o domínio padrão do GitHub. O apontamento
> de domínio personalizado (CNAME) será configurado em uma etapa futura.