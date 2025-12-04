# 🎯 Wilson Portfólio

Portfólio pessoal moderno e responsivo desenvolvido com **Angular 20**, apresentando projetos, skills e informações de contato. Destaca-se por animações suaves, design responsivo e melhor experiência do usuário.

## 📋 Sumário

- [Sobre](#sobre)
- [Tecnologias](#-tecnologias)
- [Funcionalidades](#-funcionalidades)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Começar](#-como-começar)
- [Comandos Disponíveis](#-comandos-disponíveis)
- [Responsividade](#-responsividade)
- [Segurança](#-segurança)
- [Deploy](#-deploy)

---

## Sobre

Este projeto é um portfólio profissional completo que exibe:
- **Introdução e apresentação** com descrição profissional
- **Resumo de experiência e projetos** com detalhes técnicos
- **Seção Sobre** com informações pessoais e background
- **Formulário de contato** com validação e sanitização
- **Navegação intuitiva** com menu lateral responsivo
- **Animações suaves** entre transições de componentes

---

## 🛠 Tecnologias

### Frontend
| Tecnologia | Versão | Uso |
|------------|--------|-----|
| **Angular** | 20.0.0 | Framework principal |
| **TypeScript** | 5.x | Linguagem tipada |
| **SCSS** | - | Estilização avançada |
| **RxJS** | 7.8.0 | Programação reativa |
| **Angular Router** | 20.0.0 | Roteamento entre páginas |
| **Angular Forms** | 20.0.0 | Validação de formulários |

### Ferramentas de Desenvolvimento
| Ferramenta | Uso |
|-----------|-----|
| **Angular CLI** | Scaffolding e build |
| **Prettier** | Formatação de código |
| **TypeScript Compiler** | Transpilação TS → JS |
| **Karma** | Testes unitários |

### Build & Deployment
| Ferramenta | Uso |
|-----------|-----|
| **Webpack** (via Angular) | Bundling |
| **Terser** | Minificação JS |
| **CSSO** | Minificação CSS |
| **Source Maps** | Debugging em produção |

---

## ✨ Funcionalidades

### 🎨 **Componentes Principais**

#### 1. **Navegation (Menu Lateral)**
- Menu lateral fixo com perfil do usuário
- Foto de perfil com bordas arredondadas
- Links de navegação com rota ativa (`routerLinkActive`)
- **Responsivo**: Hamburger menu em telas ≤ 450px
- Transição suave de menu (slide-in)

#### 2. **Inicial (Hero Section)**
- Apresentação pessoal com título e descrição
- Lista de skills com estilo badge
- Botões de ação (CTA)
- Efeito de animação ao carregar

#### 3. **Resumo (Portfolio)**
- Grade de cards com projetos
- Imagens de projeto
- Título e descrição
- Botões de ação
- Layout responsivo (grid adapta)

#### 4. **Sobre (About)**
- Biografia completa
- Informações profissionais
- Histórico e achievements
- Listas de competências
- Links para redes sociais

#### 5. **Contato (Contact)**
- Formulário de contato
- Validação de campos
- Mensagens de erro claras
- Botões de ação
- Sanitização de entrada

### 🚀 **Funcionalidades Avançadas**

#### **Animações de Transição**
- `fadeInUp` (0.7s): Componentes aparecem com fade + slide
- Reiniciam a cada mudança de rota
- Suave e imperceptível

#### **Roteamento Inteligente**
- Rotas: `/inicio`, `/resumo`, `/sobre`, `/contato`
- Lazy loading (opcional)
- Route guards ready
- Integração com menu de navegação

#### **Responsividade Profissional**
- Breakpoints: 1235px, 900px, 870px, 720px, 450px
- Mobile-first design
- Menu hamburger em telas pequenas
- Imagens otimizadas
- Fonts responsivas

#### **SEO & Performance**
- Meta tags estruturadas
- Lang attribute (`pt-BR`)
- Descrição e keywords
- Open Graph tags
- Preload de recursos críticos

#### **Acessibilidade**
- ARIA labels
- Semantic HTML
- Contraste de cores
- Skip links
- Focus management

### 🔒 **Segurança**

#### **Headers de Segurança**
```html
<!-- CSP contra XSS -->
<meta http-equiv="Content-Security-Policy" content="...">

<!-- Clickjacking protection -->
<meta http-equiv="X-Frame-Options" content="SAMEORIGIN">

<!-- MIME sniffing prevention -->
<meta http-equiv="X-Content-Type-Options" content="nosniff">
```

#### **Proteções Implementadas**
- XSS Prevention (Angular sanitization)
- CORS ready
- Strict TypeScript mode
- Input validation
- Output encoding

---

## 📁 Estrutura do Projeto

```
wilson-portifolio/
├── src/
│   ├── app/
│   │   ├── components/
│   │   │   ├── navegation/          # Menu lateral com perfil
│   │   │   ├── inicial/             # Hero section
│   │   │   ├── resumo/              # Portfólio/Projetos
│   │   │   ├── sobre/               # About
│   │   │   └── contato/             # Formulário de contato
│   │   ├── diretivas/
│   │   │   └── infinite-scroll.ts   # Scroll navigation
│   │   ├── app.ts                   # Componente raiz
│   │   ├── app.html                 # Template principal
│   │   ├── app.scss                 # Estilos globais
│   │   └── app.routes.ts            # Configuração de rotas
│   ├── styles/
│   │   └── variaveis.style.scss     # Variáveis globais
│   ├── index.html                   # HTML principal
│   ├── styles.scss                  # Estilos globais
│   └── main.ts                      # Entry point
├── public/                          # Ativos estáticos
├── angular.json                     # Config Angular CLI
├── tsconfig.json                    # Config TypeScript
├── package.json                     # Dependências
├── .gitignore                       # Git ignore rules
├── .eslintrc.json                   # ESLint config
└── README.md                        # Este arquivo
```

---

## 🚀 Como Começar

### Pré-requisitos
- **Node.js** 18+ (LTS recomendado)
- **npm** 9+ ou **yarn** 3+
- **Git**

### Instalação

```bash
# 1. Clone o repositório
git clone https://github.com/wilsonrogerio/Portifolio-Pessoal.git
cd wilson-portifolio

# 2. Instale dependências
npm install

# 3. Configure variáveis de ambiente (opcional)
cp .env.example .env
# Edite .env com seus valores

# 4. Inicie o servidor de desenvolvimento
npm start
```

Abra `http://localhost:4200/` no navegador. A aplicação recarregará automaticamente ao modificar arquivos.

---

## 📌 Comandos Disponíveis

### Desenvolvimento
```bash
# Servidor de desenvolvimento
npm start
# ou
ng serve

# Abra http://localhost:4200 no navegador
```

### Build
```bash
# Build para produção
npm run build

# Arquivos compilados em dist/wilson-portifolio/browser/
```

### Testes
```bash
# Testes unitários
npm test

# Com watch mode
ng test --watch

# Com coverage
ng test --code-coverage
```

### Linting & Formatação
```bash
# Verificar ESLint
ng lint

# Formatar com Prettier
npx prettier --write src/
```

### Outros
```bash
# Gerar novo componente
ng generate component nome-componente

# Gerar novo serviço
ng generate service nome-servico

# Ver versão do Angular
ng version
```

---

## 📱 Responsividade

### Breakpoints Implementados

| Breakpoint | Dispositivo | Alterações |
|-----------|-----------|-----------|
| **≥ 1235px** | Desktop Large | Layout padrão, nav fixo |
| **900px - 1235px** | Desktop | Nav 30% reduzido |
| **870px - 900px** | Tablet Large | Nav 15% reduzido |
| **720px - 870px** | Tablet | Nav no topo (15% altura) |
| **≤ 450px** | Mobile | Menu hamburger, overlay |

### Features Responsivas
- Menu hamburger com animação (≤ 450px)
- Grid de projetos adapta
- Imagens otimizadas
- Texto reescala automaticamente
- Toque/Gestos suportados

---

## 🔒 Segurança

### Medidas Implementadas
✅ **Content Security Policy (CSP)** - Previne XSS  
✅ **X-Frame-Options** - Previne clickjacking  
✅ **X-Content-Type-Options** - MIME sniffing protection  
✅ **Validação de input** - Formulários seguros  
✅ **TypeScript Strict** - Type safety  
✅ **Sanitização** - Angular DomSanitizer  
✅ **.env não versionado** - Credenciais seguras  

---

## 🚀 Deploy

### Opções de Deployment

#### **Vercel (Recomendado)**
```bash
npm install -g vercel
vercel
```

#### **Netlify**
```bash
npm install -g netlify-cli
netlify deploy --prod --dir=dist/wilson-portifolio/browser
```

#### **GitHub Pages**
```bash
npm install -g angular-cli-ghpages
ng build --configuration production --base-href=/Portifolio-Pessoal/
ngh --dir=dist/wilson-portifolio/browser
```

#### **Servidor Próprio (Node/Express)**
```bash
# Build
npm run build

# Servidor Express
node server.js
```

---

## 📈 Performance

### Otimizações Implementadas
- Angular Standalone Components (sem módulos)
- Tree-shaking automático
- Code splitting por rota
- Lazy loading pronto
- Image optimization ready
- CSS minification
- JS minification (Terser)

### Métricas (Esperadas)
- **Lighthouse Performance**: 90+
- **Bundle Size**: ~150KB (gzipped)
- **Time to Interactive**: < 2s
- **First Contentful Paint**: < 1.5s

---

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Add nova-feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

---

## 📝 Licença

Este projeto está sob a licença MIT - veja o arquivo LICENSE para detalhes.

---

## 👤 Autor

**Wilson Oliveira**
- GitHub: [@wilsonrogerio](https://github.com/wilsonrogerio)
- Email: seu.email@example.com
- Portfólio: [seu-site.com](https://seu-site.com)

---

## 📧 Suporte

Para dúvidas ou sugestões:
- Abra uma [Issue](https://github.com/wilsonrogerio/Portifolio-Pessoal/issues)
- Entre em contato via formulário no portfólio
- Email: seu.email@example.com

---

## 🙏 Agradecimentos

- [Angular Team](https://angular.io)
- [TypeScript](https://www.typescriptlang.org/)
- [SCSS](https://sass-lang.com/)
- Comunidade open source

---

**Versão**: 1.0.0  
**Última atualização**: Dezembro 2025  
**Status**: ✅ Em produção
