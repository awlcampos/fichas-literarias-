# 📚 Fichas Literárias

Catálogo pessoal de leituras — um app web progressivo para registrar, organizar e acompanhar livros lidos ao longo do tempo.

**Acesse:** [awlcampos.github.io/fichas-literarias](https://awlcampos.github.io/fichas-literarias)

---

## ✨ Funcionalidades

### 📊 Dashboard
- Meta anual de leitura com barra de progresso
- Cards rápidos: total de livros lidos, nota média, notas 10, lidos no ano
- Gráfico de livros por mês e pizza de gêneros
- Grid de capas dos livros nota 10
- Últimas fichas adicionadas

### 📚 Estante
- Catálogo visual em grid com capa, título, autor e nota
- Filtros por gênero gerados automaticamente
- Badges de status: Não lido / Want / Físico ✓
- Lixeira com restauração — nada é excluído permanentemente sem querer

### 📋 Ficha de Leitura
- Campos completos: título, autor, anos, gênero, páginas, formato, data
- Classificação: nota de 1 a 10, registro de linguagem, densidade do conteúdo
- Personagens centrais, secundários e outros
- Resumo objetivo e registro pessoal do leitor
- Toggle **Lido / Não lido** — fichas não lidas têm campos opcionais
- Seção **Acervo**: registra se tem o físico ou se quer comprar
- Upload de capa ou busca automática por **ISBN** (Google Books + Open Library)
- Impressão em **A4** com escala automática

### 🛒 Want List
- Lista de livros que quer comprar no físico
- Busca rápida por título ou autor — ideal para usar no celular num sebo
- Faixas de preço configuráveis por livro
- Botão "Comprei!" marca como físico e remove da lista automaticamente

---

## ☁️ Armazenamento

Os dados são salvos no **Google Drive** da conta da leitora, em:

```
Meu Drive > Projetos > Fichas Literárias > fichas-literarias (planilha)
```

- Cada ficha é uma linha na planilha — editável diretamente no Google Sheets
- Capas enviadas por upload ficam numa subpasta `capas/` no Drive
- Backup adicional via exportação em **Excel (.xlsx)** ou **JSON**

---

## 📱 Instalação como App (PWA)

O site pode ser instalado como aplicativo sem precisar de loja:

- **Android (Chrome):** banner "Adicionar à tela inicial" aparece automaticamente
- **iPhone/iPad (Safari):** menu compartilhar → "Adicionar à Tela de Início"
- **PC (Chrome/Edge):** ícone de instalação na barra de endereço

Funciona offline após a primeira visita.

---

## 🗂️ Estrutura do repositório

```
fichas-literarias/
├── index.html        ← app completo (HTML + CSS + JS em arquivo único)
├── manifest.json     ← configuração PWA
├── sw.js             ← service worker (cache offline)
└── icons/
    ├── icon-180.png
    ├── icon-192.png
    └── icon-512.png
```

---

## 🔄 Versionamento

| Versão | Destaques |
|--------|-----------|
| v5 | Dashboard, Want List, Acervo físico, Lido/Não lido, reescrita limpa |
| v4 | Google Sheets, PWA, Estante, Lixeira com restauração |
| v3 | Catálogo visual, filtros por gênero, impressão A4 |
| v2 | localStorage, import/export Excel e JSON, ISBN |
| v1 | Formulário de ficha, bolinhas de classificação |

---

## 🚀 Roadmap

- [ ] Dashboard com estatísticas avançadas
- [ ] Fichas de filmes (mesma base)
- [ ] Multi-usuário com acervo compartilhado
- [ ] Busca global por texto nas fichas

---

## 🛠️ Tecnologias

- HTML + CSS + JavaScript puro — sem frameworks
- [SheetJS](https://sheetjs.com/) — leitura e escrita de arquivos Excel
- [Google Sheets API](https://developers.google.com/sheets) — banco de dados na nuvem
- [Google Books API](https://developers.google.com/books) + [Open Library](https://openlibrary.org/developers) — busca por ISBN
- [GitHub Pages](https://pages.github.com/) — hospedagem gratuita

---

*Projeto desenvolvido com 💜 para registrar cada leitura com carinho.*
