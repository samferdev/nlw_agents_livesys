# NLW Agents

Este projeto foi desenvolvido durante o evento NLW da Rocketseat.

## Tecnologias e Bibliotecas Utilizadas

- **React**: Biblioteca principal para construção da interface.
- **Vite**: Ferramenta de build e desenvolvimento rápido.
- **TypeScript**: Tipagem estática para JavaScript.
- **React Router DOM**: Gerenciamento de rotas SPA.
- **@tanstack/react-query**: Gerenciamento de estado assíncrono e cache de dados.
- **TailwindCSS**: Utilitário para estilização rápida e responsiva.
- **@radix-ui/react-slot**: Composição avançada de componentes.
- **lucide-react**: Ícones SVG para React.
- **class-variance-authority, clsx, tailwind-merge**: Utilitários para manipulação de classes CSS.
- **tw-animate-css**: Animações utilitárias para Tailwind.
- **@vitejs/plugin-react, @tailwindcss/vite**: Plugins para integração do React e Tailwind com o Vite.
- **@biomejs/biome**: Linter e formatter para o código.

## Padrões de Projeto

- **Componentização**: Uso extensivo de componentes reutilizáveis.
- **Hooks**: Gerenciamento de estado e efeitos colaterais com hooks do React.
- **Alias de Imports**: Utilização de `@` como atalho para o diretório `src`.
- **Separação de páginas e componentes**: Estrutura clara entre páginas e componentes de UI.

## Setup e Configuração

1. **Clone o repositório**
   ```bash
   git clone <url-do-repo>
   cd <pasta-do-projeto>
   ```

2. **Instale as dependências**
   ```bash
   npm install
   ```

3. **Rodando o projeto em modo desenvolvimento**
   ```bash
   npm run dev
   ```

4. **Build para produção**
   ```bash
   npm run build
   ```

5. **Preview do build**
   ```bash
   npm run preview
   ```

## Observações

- O projeto utiliza TailwindCSS, já configurado e importado em `src/index.css`.
- O Vite está configurado para usar plugins do React e Tailwind, além de alias para facilitar os imports.
- Para garantir a qualidade do código, utilize o Biome (`npx biome check .`). 