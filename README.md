<h1 align="center">Beyond Bits</h1>

<p align="center">
  <strong>A fusão entre mente e máquina — entre a página em branco e a invenção.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-em%20evolução-blue?style=flat-square" alt="status">
  <img src="https://img.shields.io/badge/licença-MIT-green?style=flat-square" alt="licença">
  <img src="https://img.shields.io/badge/stack-JS%20%7C%20PHP%20%7C%20SQL-lightgrey?style=flat-square" alt="stack">
</p>

---

## Visão Geral

Não entregamos apenas sistemas ou layouts. Construímos marcas e experiências digitais com sofisticação, clareza e precisão técnica.

A Beyond Bits une inteligência artificial, design editorial refinado e engenharia de software para criar produtos modernos, escaláveis e **sem lock-in** — o cliente é dono do código, dos dados e das decisões de arquitetura.

### O que fazemos

| Frente | Escopo |
|---|---|
| **Desenvolvimento de sistemas** | Aplicações web, integrações e sustentação |
| **Gestão de projetos** | Levantamento de requisitos, roadmap e entrega |
| **Design e experiência** | Identidade visual, UI e design editorial |
| **Suporte técnico** | Manutenção evolutiva e corretiva |

---

## Arquitetura do Repositório

```
beyond/
├── assets/     # Mídias visuais: imagens, ícones, vídeos demonstrativos
├── docs/       # Documentação técnica, requisitos e decisões de arquitetura
├── src/        # Código-fonte: componentes, controladores e lógica de domínio
│   ├── css/    # Estilização, temas e tokens visuais
│   └── js/     # Comportamento, integrações e manipulação de interface
└── README.md
```

| Diretório | Responsabilidade | Não colocar aqui |
|---|---|---|
| `/assets` | Mídia final otimizada | Arquivos-fonte (`.psd`, `.fig`, `.ai`) |
| `/docs` | ADRs, especificações, guias | Anotações temporárias |
| `/src` | Código de aplicação | Build gerado, `node_modules` |
| `/src/css` | Estilos e temas | CSS inline duplicado |
| `/src/js` | Scripts e integrações | Credenciais ou chaves de API |

---

## Guia de Assets Visuais

### Padrões técnicos

| Critério | Especificação |
|---|---|
| Imagens estáticas | `PNG` (com transparência) ou `JPG` (fotografia) |
| Elementos animados | `MP4` (H.264) ou `WebM` |
| Ícones | `SVG` otimizado |
| Banners e hero | 16:9 — `1280x720` ou `1920x1080` px |
| Peso máximo por arquivo | **500 KB** |
| Nomenclatura | `kebab-case`, descritiva, sem acento |

### Assets essenciais

| Arquivo | Descrição |
|---|---|
| `logo-beyond-bits.png` | Logo em versões *dark* e *light*, fundo transparente |
| `hero-biomechanical-bg.png` | Fundo principal da área hero (imagem ou vídeo) |
| `showcase-project-preview.png` | Previews de projetos e cases |
| `icon-brain-hybrid.svg` | Ícone da inteligência híbrida |

---

## Stack

### Linguagens

| JavaScript | PHP | HTML | CSS | C |
|:---:|:---:|:---:|:---:|:---:|
| <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/JavaJs.png" alt="JavaScript" width="110"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/PHP.png" alt="PHP" width="110"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/HTML.png" alt="HTML" width="70"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/CSS.png" alt="CSS" width="110"> | <img src="https://raw.githubusercontent.com/beyondBitsLtda/beyond/main/img/3765627-removebg-preview.png" alt="C" width="90"> |

### Ferramentas

| SQL Server | MySQL | Figma | Git |
|:---:|:---:|:---:|:---:|
| <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/sql%20server.png" alt="SQL Server" width="110"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/MYSQL.png" alt="MySQL" width="110"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/FIGMA.png" alt="Figma" width="70"> | <img src="https://raw.githubusercontent.com/bryansf94/bryansf94/main/img/GIT.png" alt="Git" width="90"> |

---

## Padrões de Contribuição

### Commits

Padrão **Conventional Commits**:

```
<tipo>(<escopo opcional>): <descrição no imperativo>
```

| Tipo | Uso |
|---|---|
| `feat` | Nova funcionalidade |
| `fix` | Correção de defeito |
| `docs` | Documentação |
| `style` | Formatação sem alteração de comportamento |
| `refactor` | Reestruturação de código |
| `perf` | Ganho de performance |
| `test` | Testes |
| `chore` | Build, dependências, configuração |

```bash
feat(auth): adiciona validação de sessão expirada
fix(form): corrige envio duplicado no submit
docs(readme): atualiza guia de assets
```

### Branches

```
main              # Produção — protegida, sem commit direto
develop           # Integração
feat/<nome>       # Nova funcionalidade
fix/<nome>        # Correção
docs/<nome>       # Documentação
```

### Pull Requests

Todo PR deve conter:

- [ ] Descrição objetiva do que foi alterado e **por quê**
- [ ] Referência à issue relacionada (`Closes #00`)
- [ ] Evidência visual (print ou GIF) quando houver mudança de interface
- [ ] Testes manuais descritos ou automatizados executados
- [ ] Sem credenciais, tokens ou dados sensíveis no diff
- [ ] Revisão aprovada por pelo menos 1 mantenedor

### Boas práticas de código

- Código legível antes de código esperto — nome de variável vale mais que comentário.
- Comentar o **porquê**, não o **o quê**.
- Zero dependência sem justificativa: cada pacote novo é dívida técnica.
- Sem segredos no repositório. Use `.env` e mantenha `.env.example` versionado.
- Arquivos de build, cache e `node_modules` ficam no `.gitignore`.

---

## Como rodar localmente

```bash
git clone https://github.com/beyondBitsLtda/beyond.git
cd beyond
```

Para projetos estáticos, sirva a pasta com qualquer servidor local:

```bash
npx serve .
```

---

<p align="center">
  <img width="1000" src="img/github-snake.svg" alt="Contribuições">
</p>

<p align="center">
  <sub>Beyond Bits — criatividade é conectar pessoas, ideias e tecnologia.</sub>
</p>
