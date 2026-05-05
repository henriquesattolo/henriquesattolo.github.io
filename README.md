# henriquesattolo.github.io

🌐 Site portfólio profissional hospedado no **GitHub Pages** — vitrine para os recrutadores.

> Substitui os repos antigos `ISoftware` (2020) e `hello-world` (2019) que não representam mais o nível atual.

## Stack

- **HTML5 + CSS3** estático (sem framework pesado)
- **GitHub Pages** — hospedagem grátis em `henriquesattolo.github.io`
- **GitHub Actions** — deploy automático no push
- **Lighthouse CI** — garante performance > 90

## Por que ter um portfólio

Recrutadores não leem todos os 9 repos de DevOps. O portfólio resume **em 30 segundos**:

1. Quem você é (12 anos de infra → DevOps)
2. O que faz (stack, certificações)
3. Provas (links pros repos certos)
4. Contato (LinkedIn, email)

## Seções do site

| Seção | Conteúdo |
|---|---|
| Hero | Foto + título + 1 frase de pitch |
| Stack | Ícones de Docker, K8s, Terraform, Ansible, AWS, etc |
| Projetos | Cards dos 5 melhores repos com screenshots |
| Sobre | Trajetória profissional resumida |
| Contato | LinkedIn, email, GitHub |

## Estrutura planejada

```
henriquesattolo.github.io/
├── index.html
├── styles.css
├── assets/
│   ├── img/
│   └── icons/                  # SVGs da stack
├── projects.json               # data dos cards
├── .github/workflows/
│   ├── deploy.yml              # publica no GitHub Pages
│   └── lighthouse.yml          # checa performance em PR
└── README.md
```

## Como ativar GitHub Pages

1. **Settings** do repositório
2. **Pages** (no menu lateral)
3. Em **Source**: escolha `Deploy from a branch` → branch `main` → folder `/ (root)`
4. Salve. Em ~1min o site estará no ar em https://henriquesattolo.github.io

Para deploy via GitHub Actions (mais flexível), troque o Source para "GitHub Actions" e use o workflow `.github/workflows/deploy.yml`.

## Diferenciais planejados

- ✅ **Performance 100/100** no Lighthouse (HTML estático puro)
- ✅ **Mobile-first** responsivo
- ✅ **Modo escuro** automático (via `prefers-color-scheme`)
- ✅ **JSON-LD** estruturado para SEO
- ✅ **Open Graph** para preview no LinkedIn

## Próximos passos

- [ ] Criar `index.html` com seção Hero
- [ ] Adicionar cards de projetos (gerados a partir de `projects.json`)
- [ ] Configurar GitHub Action de deploy
- [ ] Tirar screenshots dos repos mais relevantes
- [ ] Adicionar ícones SVG da stack
- [ ] Configurar domínio personalizado (opcional)

## Autor

**Henrique Sattolo** — [github.com/henriquesattolo](https://github.com/henriquesattolo) — [LinkedIn](https://www.linkedin.com/in/henrique-sattolo-84a02ba8/)
