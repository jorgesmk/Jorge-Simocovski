# Portfólio — Jorge Simocovski

Este é um portfólio em Jekyll hospedado no GitHub Pages, refatorado para eliminar paginação desnecessária e manter a estrutura limpa e eficiente.

## Estrutura do Projeto

```
_pages/
  index.md              # Home
  about.md              # Sobre
  experience.md         # Experiência (timeline)
  skills.md             # Skills (badges)
  cases.md              # Index de cases
  *.md                  # Case detail pages

_data/
  navigation.yml        # Navegação do site

_includes/
  site-nav.html         # Navegação (incluso em todas as páginas)

assets/css/
  custom.css            # Design system (Navy #003366 + Laranja #FF5F1F)

_layouts/
  single.html           # Layout padrão (limpo, sem paginação)
```

## Como Adicionar um Novo Case

1. Crie um novo arquivo markdown em `_pages/` (ex: `_pages/seu-case.md`)
2. Use o front matter com permalink `/cases/seu-case/`:
   ```yaml
   ---
   title: "Título do Case"
   permalink: /cases/seu-case/
   layout: single
   author_profile: false
   ---
   ```
3. Estruture o conteúdo: Context → Problem → Decision → Approach → Metrics → Impact → Result
4. Adicione um link no `cases.md` para referência cruzada
5. Commit e push!

## Paleta de Cores

- **Primária (Navy):** `#003366` — backgrounds, títulos, elementos principais
- **Destaque (Laranja):** `#FF5F1F` — botões, números de impacto, links de ação
- **Background:** `#FFFFFF` ou `#F8F9FA` (cinza claro)
- **Texto:** `#1A1A1A` (escuro) ou `#555555` (médio)

Todas as cores estão definidas em `assets/css/custom.css` como variáveis CSS (`:root`).

## Testar Localmente

```powershell
gem install bundler jekyll
bundle install
bundle exec jekyll serve --livereload
```

Acesse `http://localhost:4000/Jorge-Simocovski/` no navegador.

## Commits e Deploy

- Commits semânticos: feature, fix, refactor, docs, style
- Cada push para `main` dispara build automático no GitHub Pages (~1 minuto de propagação)
- Rollbacks são fáceis via git revert

