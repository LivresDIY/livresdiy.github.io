# Livres DIY - Landing Page

Este é o repositório do website da comunidade **Livres DIY**, uma moderna landing page dedicada à criação de um ecossistema de liberdade digital através de tecnologias descentralizadas, privacidade e projetos DIY.

## 🎨 Características da Landing Page

- ✨ **Design Moderno**: Landing page profissional com gradientes e animações
- 📱 **Totalmente Responsiva**: Otimizada para desktop, tablet e mobile
- ⚡ **Performance Otimizada**: CSS customizado sem dependências externas
- 🎯 **Foco em Conversão**: CTAs estratégicos e hierarquia visual clara
- 📝 **Fácil de Editar**: Sistema de gerenciamento de conteúdo baseado em YAML

## 📋 Informações Técnicas

### Tecnologias Utilizadas
- **Jekyll** - Gerador de sites estáticos
- **GitHub Pages** - Hospedagem gratuita
- **CSS Custom** - Design landing page personalizado (sem tema externo)
- **YAML** - Gerenciamento de conteúdo estruturado
- **Markdown** - Formatação de conteúdo
- **SCSS** - Estilização avançada com variáveis CSS

### Estrutura do Projeto
```
livres-website/
├── _config.yml          # Configurações do site
├── _data/
│   └── content.yml      # Conteúdo estruturado (NOVO!)
├── _includes/           # Seções reutilizáveis
│   ├── hero-section.md
│   ├── middle-section.md
│   └── bottom-section.md
├── _layouts/
│   └── landing.html     # Layout da landing page (NOVO!)
├── assets/
│   └── main.scss        # Estilos customizados da landing page
├── index.md             # Página principal (atualizada)
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

Este site usa um **sistema modular de conteúdo** que torna super fácil fazer alterações. Não se preocupe - você não precisa saber programação!

### 📝 Onde Está o Conteúdo

O conteúdo é gerenciado através de **dois sistemas complementares**:

#### 1. **Arquivo Principal de Conteúdo** (`_data/content.yml`)
Este é o arquivo **mais importante** - aqui você pode alterar:
- Títulos e subtítulos
- Textos dos botões e links
- Lista de recursos/funcionalidades
- Links das redes sociais
- Todas as frases principais

#### 2. **Seções de Template** (`_includes/`)
Arquivos que controlam a estrutura:
- **`hero-section.md`** - Seção do topo (título principal)
- **`middle-section.md`** - Seção do meio (conteúdo principal)  
- **`bottom-section.md`** - Seção inferior (call-to-action)

### ✏️ Como Editar

#### Opção 1: Editar Diretamente no GitHub (Mais Fácil)

**Para editar o conteúdo principal (RECOMENDADO):**
1. **Acesse o repositório**: Vá para https://github.com/LivresDIY/livres-website
2. **Navegue até**: `_data/` → `content.yml`
3. **Clique no ícone do lápis** (✏️) no canto superior direito
4. **Faça suas alterações** no formato YAML (veja exemplos abaixo)
5. **Salve as mudanças**: Role para baixo, adicione uma descrição e clique em "Commit changes"

**Para editar a estrutura (avançado):**
1. **Navegue até a pasta**: `_includes/`
2. **Escolha o arquivo**: Clique no arquivo que deseja editar (ex: `hero-section.md`)
3. **Siga os mesmos passos** de edição

**🎯 As mudanças aparecerão no site automaticamente em alguns minutos!**

#### Opção 2: Usando um Editor de Texto Local

1. **Baixe os arquivos**: Faça download do repositório como ZIP
2. **Edite com qualquer editor**: Use Notepad, Word, ou qualquer editor de texto
3. **Envie de volta**: Faça upload dos arquivos editados

### 📖 Guia de Formatação

#### YAML (Para editar `_data/content.yml`)

O YAML é um formato simples para dados estruturados. **Use espaços, não tabs!**

```yaml
# Comentários começam com #
titulo: "Seu título aqui"
subtitulo: "Seu subtítulo aqui"

# Para textos longos, use |
descricao: |
  Este é um texto longo
  que pode ter várias linhas
  e parágrafos.

# Para listas
recursos:
  - titulo: "Primeiro recurso"
    descricao: "Descrição do primeiro recurso"
  - titulo: "Segundo recurso"
    descricao: "Descrição do segundo recurso"

# Para links
botao_texto: "Clique aqui"
botao_link: "#secao"
```

#### Markdown (Para editar arquivos `.md`)

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

### ✨ Alterando o Título Principal e Botão
**Arquivo**: `_data/content.yml` - Seção `hero:`

```yaml
hero:
  title: "Seu Novo Título Aqui!"
  subtitle: "Sua nova descrição da comunidade aqui."
  button_text: "Novo Texto do Botão"
  button_link: "#nova-secao"
```

### 🔧 Adicionando/Editando Recursos da Lista
**Arquivo**: `_data/content.yml` - Seção `middle: → features:`

```yaml
middle:
  features:
    - title: "Novo Recurso"
      description: "Descrição do seu novo recurso aqui"
    - title: "Blockchain"
      description: "Desenvolvimento com tecnologias blockchain"
    - title: "Inteligência Artificial"
      description: "Projetos com IA e machine learning"
```

### 🔗 Atualizando Links Sociais
**Arquivo**: `_data/content.yml` - Seção `social:`

```yaml
social:
  linkedin: "https://linkedin.com/company/seuperfil"
  discord: "https://discord.gg/seuservidor"
  # Adicione mais redes se necessário:
  # twitter: "https://twitter.com/seuperfil"
  # instagram: "https://instagram.com/seuperfil"
```

### 📝 Alterando o Call-to-Action Final
**Arquivo**: `_data/content.yml` - Seção `bottom:`

```yaml
bottom:
  title: "Novo título da seção final!"
  description: |
    Seu novo texto aqui.
    
    Pode ter múltiplos parágrafos.
    
    E chamadas para ação personalizadas.
  cta_text: "Novo Botão!"
  cta_link: "#contato"
```

### 🎨 Exemplo: Mudança Completa do Hero
**Antes:**
```yaml
hero:
  title: "Construa o futuro que deseja viver. Seja Livres!"
  subtitle: "Livres é uma comunidade..."
  button_text: "Conheça Livres"
  button_link: "#about"
```

**Depois:**
```yaml
hero:
  title: "Transforme Ideias em Realidade!"
  subtitle: "Junte-se à maior comunidade de criadores digitais do Brasil. Aprenda, construa e compartilhe projetos incríveis."
  button_text: "Começar Agora"
  button_link: "#comece"
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

## 🎨 Recursos da Landing Page

### ✨ Design Profissional
- **Hero Section**: Seção de destaque com gradiente e call-to-action
- **Cards Interativos**: Lista de recursos com hover effects
- **Botões Animados**: CTAs com transformações e sombras
- **Tipografia Moderna**: Hierarquia visual clara e legível

### 📱 Responsividade Total
- **Desktop**: Layout completo com todas as funcionalidades
- **Tablet**: Adaptação otimizada para telas médias  
- **Mobile**: Interface simplificada para smartphones

### ⚡ Performance
- **CSS Customizado**: Sem dependências externas de temas
- **Otimização de Carregamento**: Estilos inline e minificados
- **SEO Friendly**: Meta tags e estrutura semântica

---

## 🚀 Publicação e Deploy

O site é automaticamente publicado no **GitHub Pages** sempre que você faz alterações na branch `main`. Não é necessário fazer nada extra - as mudanças aparecem automaticamente em alguns minutos!

**URL do Site**: https://livres.diy

### 🔄 Processo de Atualização
1. **Edite o conteúdo** (principalmente `_data/content.yml`)
2. **Commit as mudanças** no GitHub
3. **Aguarde 2-5 minutos** para o deploy automático
4. **Verifique o resultado** no site ao vivo

---

## 🆘 Precisa de Ajuda?

### 📚 Recursos de Aprendizado
1. **Consulte os tutoriais** listados acima
2. **Pratique no arquivo de teste** antes de fazer mudanças definitivas
3. **Use o preview** do GitHub para ver suas alterações YAML

### 💬 Suporte
- **Abra uma issue** no GitHub descrevendo seu problema
- **Entre em contato** através do email: contato@livres.diy
- **Consulte a documentação** do Jekyll para dúvidas avançadas

### ⚠️ Dicas Importantes
- **Sempre use espaços** (não tabs) em arquivos YAML
- **Teste localmente** se possível antes de fazer commit
- **Faça backup** do conteúdo antes de grandes mudanças
- **Commits pequenos** são mais fáceis de reverter se necessário

---

## 📄 Licença

Este projeto está sob a licença especificada no arquivo `LICENSE`.

---

## 🏗️ Arquitetura do Projeto

### Fluxo de Conteúdo
```
_data/content.yml → _includes/*.md → _layouts/landing.html → index.md → Site Final
```

### Tecnologias Integradas
- **Jekyll**: Processamento e build
- **YAML**: Gerenciamento de dados
- **Markdown**: Formatação de conteúdo  
- **SCSS**: Estilização avançada
- **GitHub Pages**: Deploy automático

---

**Feito com ❤️ pela comunidade Livres DIY**  
*Transformando ideias em realidade digital desde 2025*