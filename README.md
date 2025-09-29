# Livres DIY - Website

Este é o repositório do website da comunidade **Livres DIY**, uma plataforma dedicada à criação de um ecossistema de liberdade digital através de tecnologias descentralizadas, privacidade e projetos DIY.

## 📋 Informações Técnicas

### Tecnologias Utilizadas
- **Jekyll** - Gerador de sites estáticos
- **GitHub Pages** - Hospedagem gratuita
- **Tema Minima** - Design limpo e responsivo
- **Markdown** - Formatação de conteúdo
- **SCSS** - Estilização avançada

### Estrutura do Projeto
```
livres-website/
├── _config.yml          # Configurações do site
├── _includes/           # Seções reutilizáveis
│   ├── hero-section.md
│   ├── middle-section.md
│   └── bottom-section.md
├── assets/
│   └── main.scss        # Estilos customizados
├── index.html           # Página principal
├── Gemfile             # Dependências Ruby
└── README.md           # Este arquivo
```

### Configuração Local

#### Pré-requisitos
- Ruby (versão 2.7 ou superior)
- Bundler
- Git

#### Instalação
```bash
# Clone o repositório
git clone https://github.com/LivresDIY/livres-website.git
cd livres-website

# Instale as dependências
bundle install

# Execute o servidor local
bundle exec jekyll serve

# Acesse em: http://localhost:4000
```

---

## 🎨 Como Editar o Conteúdo (Para Não-Técnicos)

Este site é dividido em **três seções principais** que você pode editar facilmente. Não se preocupe - você não precisa saber programação!

### 📝 Onde Está o Conteúdo

O conteúdo do site está dividido em 3 arquivos dentro da pasta `_includes/`:

1. **`hero-section.md`** - Seção do topo (título principal)
2. **`middle-section.md`** - Seção do meio (conteúdo principal)
3. **`bottom-section.md`** - Seção inferior (call-to-action e links)

### ✏️ Como Editar

#### Opção 1: Editar Diretamente no GitHub (Mais Fácil)

1. **Acesse o repositório**: Vá para https://github.com/LivresDIY/livres-website
2. **Navegue até a pasta**: Clique em `_includes/`
3. **Escolha o arquivo**: Clique no arquivo que deseja editar (ex: `hero-section.md`)
4. **Clique no ícone do lápis** (✏️) no canto superior direito
5. **Faça suas alterações** usando a formatação Markdown
6. **Salve as mudanças**: Role para baixo, adicione uma descrição e clique em "Commit changes"

**🎯 As mudanças aparecerão no site automaticamente em alguns minutos!**

#### Opção 2: Usando um Editor de Texto Local

1. **Baixe os arquivos**: Faça download do repositório como ZIP
2. **Edite com qualquer editor**: Use Notepad, Word, ou qualquer editor de texto
3. **Envie de volta**: Faça upload dos arquivos editados

### 📖 Guia de Formatação Markdown

O Markdown é uma linguagem simples para formatar texto. Aqui estão os comandos básicos:

```markdown
# Título Principal (H1)
## Título Secundário (H2)
### Título Terciário (H3)

**Texto em negrito**
*Texto em itálico*

• Lista com pontos
• Outro item da lista

[Texto do link](https://exemplo.com)

---
(Linha horizontal)
```

### 🔗 Tutoriais Recomendados em Português

Para aprender mais sobre como editar e gerenciar conteúdo:

1. **Markdown Básico**:
   - [Guia Markdown em Português](https://docs.pipz.com/central-de-ajuda/learning-center/guia-basico-de-markdown)
   - [Tutorial Markdown - DevMedia](https://www.devmedia.com.br/markdown-tutorial/33674)

2. **Usando o GitHub**:
   - [Como usar o GitHub - Tutorial Completo](https://www.hostinger.com.br/tutoriais/tutorial-do-git)
   - [Editando arquivos no GitHub](https://docs.github.com/pt/repositories/working-with-files/managing-files/editing-files)

3. **Jekyll e Sites Estáticos**:
   - [Jekyll em Português - Documentação](https://jekyllrb-pt.github.io/)
   - [Criando sites com Jekyll](https://www.devmedia.com.br/criando-sites-estaticos-com-jekyll/32842)

---

## 🎯 Exemplos Práticos de Edição

### Alterando o Título Principal
**Arquivo**: `_includes/hero-section.md`

```markdown
# Seu Novo Título Aqui!

Sua nova descrição da comunidade aqui.

[Texto do botão](#link)
```

### Adicionando Nova Seção de Conteúdo
**Arquivo**: `_includes/middle-section.md`

```markdown
## Novo Tópico

Seu conteúdo aqui com **texto em negrito**.

• Primeiro item da lista
• Segundo item da lista
• Terceiro item da lista

[Link para mais informações](https://exemplo.com)
```

### Atualizando Links Sociais
**Arquivo**: `_includes/bottom-section.md`

```markdown
<!-- Substitua os links pelos seus próprios -->
[LinkedIn](https://linkedin.com/company/seuperfil) | [Discord](https://discord.gg/seuservidor)
```

---

## ⚙️ Configurações do Site

Para alterar informações básicas do site (título, descrição, etc.), edite o arquivo `_config.yml`:

```yaml
title: Livres DIY
email: contato@livres.diy
description: >-
  Sua nova descrição aqui
url: "https://livres.diy"
twitter_username: seuperfil
github_username: SeuUsuario
```

**⚠️ Importante**: Após alterar `_config.yml`, o site pode levar alguns minutos para atualizar.

---

## 🚀 Publicação e Deploy

O site é automaticamente publicado no **GitHub Pages** sempre que você faz alterações na branch `main`. Não é necessário fazer nada extra - as mudanças aparecem automaticamente em alguns minutos!

**URL do Site**: https://livres.diy

---

## 🆘 Precisa de Ajuda?

Se você encontrar dificuldades ou tiver dúvidas:

1. **Consulte os tutoriais** listados acima
2. **Abra uma issue** no GitHub descrevendo seu problema
3. **Entre em contato** através do email: contato@livres.diy

---

## 📄 Licença

Este projeto está sob a licença especificada no arquivo `LICENSE`.

---

**Feito com ❤️ pela comunidade Livres DIY**