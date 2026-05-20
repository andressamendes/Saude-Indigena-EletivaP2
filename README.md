# ACOLHER É CUIDAR

**Infográfico interativo — POP · Receptividade e Conduta para com Pessoas em Situação de Rua na Atenção Primária à Saúde**

> Produto acadêmico da disciplina **Relações Étnico-Raciais e Saúde da População Negra e Indígena**  
> Profa. Me. Isadora Alves Cotrim · Turma XII · Faculdade Afya Guanambi · BA

---

## Tecnologias

| Tecnologia | Função |
|---|---|
| React 18 + Vite | SPA estática |
| Tailwind CSS 3 | Estilização |
| Framer Motion | Animações |
| Lucide React | Ícones |
| gh-pages | Deploy no GitHub Pages |

---

## Instalação local

```bash
# 1. Clone o repositório
git clone https://github.com/<SEU-USUARIO>/pop-acolhimento.git
cd pop-acolhimento

# 2. Instale dependências
npm install

# 3. Inicie o servidor de desenvolvimento
npm run dev
```

Abra `http://localhost:5173/pop-acolhimento/` no navegador.

---

## Adicionando a Logo

1. Copie o arquivo da logo para `public/logo-afya.png`
2. Salve com o nome **exato**: `logo-afya.png`
3. Reconstrua o projeto: `npm run build`

A logo aparece automaticamente no Hero e no Encerramento.

---

## Deploy no GitHub Pages

### Passo 1 — Ajuste o nome do repositório no Vite

Abra `vite.config.js` e altere o `base` para o nome do seu repositório:

```js
base: '/NOME-DO-SEU-REPOSITORIO/',
```

### Passo 2 — Ajuste o homepage no package.json (opcional)

```json
"homepage": "https://<SEU-USUARIO>.github.io/pop-acolhimento"
```

### Passo 3 — Deploy

```bash
npm run deploy
```

Isso executa `npm run build` e publica a pasta `dist/` na branch `gh-pages`.

### Passo 4 — Ative o GitHub Pages

No repositório: **Settings → Pages → Branch: gh-pages → / (root) → Save**

A aplicação estará disponível em:  
`https://<SEU-USUARIO>.github.io/pop-acolhimento/`

---

## Estrutura do projeto

```
pop-acolhimento/
├── public/
│   └── logo-afya.png        ← ADICIONE A LOGO AQUI
├── src/
│   ├── components/
│   │   ├── Navbar.jsx        Barra de navegação fixa
│   │   ├── Hero.jsx          Tela inicial — título e créditos
│   │   ├── Principios.jsx    6 princípios do acolhimento
│   │   ├── FluxoAcolhimento.jsx  Timeline com 5 etapas
│   │   ├── SituacoesPraticas.jsx 6 situações interativas
│   │   ├── DireitosDignidade.jsx 5 direitos fundamentais
│   │   ├── FrasesImpacto.jsx 4 frases institucionais
│   │   └── Encerramento.jsx  Créditos e mensagem final
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
└── postcss.config.js
```

---

## Seções da aplicação

| # | Seção | Conteúdo |
|---|---|---|
| 1 | **Hero** | Logo, título "ACOLHER É CUIDAR", disciplina, docente, turma |
| 2 | **Princípios** | 6 cards: Equidade, Escuta, Respeito, Vínculo, Dignidade, Red. Danos |
| 3 | **Fluxo** | Timeline com 5 etapas do acolhimento |
| 4 | **Situações Práticas** | 6 temas interativos: conduta adequada × inadequada |
| 5 | **Direitos** | 5 direitos com base legal |
| 6 | **Frases** | 4 frases de impacto institucional |
| 7 | **Encerramento** | Créditos, referências e mensagem final |

---

## Licença

Uso acadêmico · Faculdade Afya Guanambi · 2026
