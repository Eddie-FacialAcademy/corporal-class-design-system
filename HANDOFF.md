# Handoff — Corporal Class Design System (estado em 2026-06-11)

Desenvolvido por **Edegar Junior**. Ponto de retomada; atualizar conforme avançar.

## ✅ Concluído

### Design system online (GitHub Pages)
- **URL pública:** https://eddie-facialacademy.github.io/corporal-class-design-system/
- Repo público `corporal-class-design-system` (conta `Eddie-FacialAcademy`), branch `main`, `index.html` na raiz.
- Pasta dedicada local: `_Claudio x Eddie/Corporal Class - Design System/` (1 pasta por marca).
- `index.html`: showcase self-contained, dark/light automático + toggle, click-to-copy, **copiar/baixar SVG** de logos+ícones, **download PNG** dos gradientes.

### Pacote portátil (`design-system/`)
- `silka.css` · `corporal-design-system.css` · `corporal-design-tokens.json` · `Button.tsx` · `THEME.md` · `DESIGN-SYSTEM.md`.
- Gerado a partir do template **Facial Class** via recolor roxo→bordô (`#D6515C` / pantone 186 U) + rename `fc-`→`cc-`, `--roxo`→`--bordo`, `--lilas`→`--coral`.

### Marca (fiel ao brandbook §3.6)
- **Cor primária:** bordô `#D6515C` (pantone 186 U). Institucionais (5): bordô, vermelho claro `#FFB1BD`, amarelado `#FFE4A4`, branco, preto. Acento derivado coral `#E88A92`.
- **Logos** Corporal (4 composições) embutidos como `<symbol>` `currentColor` (seguem o tema: branco no dark, bordô no light).
- **Copy** revisada pra Corporal (Curso Celulite PRO · estética corporal · planos Ouro & Black).
- **Fonte** Silka inalterada (embutida base64).

## Deploy / git (durável)
- `.git` **fora do OneDrive**: `AppData\Local\gitdirs\corporal-class-design-system`.
- **LF** travado (`.gitattributes`); `.gitignore` barra `desktop.ini`.
- **Auth:** Git Credential Manager (Cofre do Windows) — push **silencioso, sem token**. Republicar: editar → `git add/commit/push`.

## 🔜 Próximo (opcional — Framer)
- Aplicar no Framer: criar **Color Styles** (Light+Dark) e **Text Styles** (L/M/S = 1200/810/390) — ver `design-system/DESIGN-SYSTEM.md` (mecânica + bug da Server API + workaround). Importar `Button.tsx`.
- Ainda não há projeto Framer / landing da Corporal Class neste setup (só o design system).

## Arquivos-chave
- Showcase: `index.html`
- Pacote portátil: `design-system/` (css, tokens.json, Button.tsx, silka.css, DESIGN-SYSTEM.md, THEME.md)
- Docs: `README.md`, `HANDOFF.md`
