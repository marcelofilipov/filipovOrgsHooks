# 📱 filipovOrgsHooks

> Aplicativo mobile para listagem e gerenciamento de organizações — desenvolvido com React Native CLI e React Hooks

[![Top Language](https://img.shields.io/github/languages/top/marcelofilipov/filipovOrgsHooks)](https://github.com/marcelofilipov/filipovOrgsHooks)
[![Repo Size](https://img.shields.io/github/repo-size/marcelofilipov/filipovOrgsHooks)](https://github.com/marcelofilipov/filipovOrgsHooks)
[![Commit Activity](https://img.shields.io/github/commit-activity/m/marcelofilipov/filipovOrgsHooks)](https://github.com/marcelofilipov/filipovOrgsHooks/commits/master)

---

## 📋 Sumário

- [Sobre o Projeto](#sobre-o-projeto)
- [Tecnologias](#tecnologias)
- [Pré-requisitos](#pré-requisitos)
- [Instalação e Execução](#instalação-e-execução)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Testes](#testes)
- [Qualidade de Código](#qualidade-de-código)
- [Contribuindo](#contribuindo)

---

## Sobre o Projeto

O **filipovOrgsHooks** é uma aplicação mobile desenvolvida com **React Native CLI** (bare workflow), focada em demonstrar o uso de **React Hooks** para gerenciamento de estado e efeitos colaterais. O app permite listar e interagir com organizações, servindo como estudo prático de componentes funcionais modernos com React Native.

> ⚠️ Este projeto utiliza o **React Native CLI** diretamente — **não** utiliza Expo. É necessário o ambiente nativo de desenvolvimento configurado (Android SDK e/ou Xcode).

---

## Tecnologias

**Core**
- **React Native** (CLI / bare workflow)
- **JavaScript** (ES6+)
- **React Hooks** (`useState`, `useEffect`, `useCallback`, entre outros)

**Build nativo**
- **Java** — módulo Android
- **Objective-C** — módulo iOS
- **Metro Bundler** — bundler JavaScript do React Native
- **Buck** — sistema de build (`.buckconfig`)

**Tooling**
- **ESLint** — análise estática de código (`.eslintrc.json`)
- **Prettier** — formatação de código (`.prettierrc.json`)
- **Yarn** — gerenciador de dependências
- **Babel** — transpilação JavaScript (`babel.config.js`)
- **Watchman** — monitoramento de arquivos (`.watchmanconfig`)

---

## Pré-requisitos

> Este projeto exige o ambiente de desenvolvimento React Native CLI completo. Siga o guia oficial antes de prosseguir: [https://reactnative.dev/docs/environment-setup](https://reactnative.dev/docs/environment-setup)

**Geral**
- **Node.js** 14 ou superior (recomendado LTS)
- **Yarn** 1.x
- **Watchman** (macOS/Linux)

**Android**
- Android Studio
- Android SDK (API 29+)
- Emulador Android ou dispositivo físico com depuração USB habilitada

**iOS** (apenas macOS)
- Xcode 12+
- CocoaPods (`sudo gem install cocoapods`)
- Simulador iOS ou dispositivo físico

---

## Instalação e Execução

**1. Clone o repositório**

```bash
git clone https://github.com/marcelofilipov/filipovOrgsHooks.git
cd filipovOrgsHooks
```

**2. Instale as dependências JavaScript**

```bash
yarn install
```

**3. Instale as dependências nativas iOS** (apenas macOS)

```bash
cd ios && pod install && cd ..
```

**4. Inicie o Metro Bundler**

```bash
yarn start
```

**5. Execute no Android**

```bash
yarn android
```

**6. Execute no iOS** (apenas macOS)

```bash
yarn ios
```

---

## Estrutura do Projeto

```
filipovOrgsHooks/
├── __tests__/             # Testes automatizados (Jest)
├── android/               # Projeto nativo Android (Java)
├── ios/                   # Projeto nativo iOS (Objective-C)
├── src/                   # Código-fonte principal
│   └── ...                # Componentes, hooks, telas, serviços
├── App.js                 # Componente raiz da aplicação
├── index.js               # Entry point — registra o componente raiz
├── app.json               # Configuração do app (nome, bundle id)
├── babel.config.js        # Configuração do Babel
├── metro.config.js        # Configuração do Metro Bundler
├── .eslintrc.json         # Regras ESLint
├── .eslintignore          # Arquivos ignorados pelo ESLint
├── .prettierrc.json       # Regras Prettier
├── .editorconfig          # Configurações de editor
├── .flowconfig            # Configuração Flow (type checker legado)
├── .buckconfig            # Configuração Buck build
├── .watchmanconfig        # Configuração Watchman
├── package.json           # Dependências e scripts npm/yarn
└── yarn.lock              # Lockfile Yarn
```

---

## Testes

O projeto utiliza **Jest** para testes, com o diretório `__tests__/` na raiz.

```bash
# Executar todos os testes
yarn test

# Executar com watch mode
yarn test --watch

# Gerar relatório de cobertura
yarn test --coverage
```

---

## Qualidade de Código

O projeto possui **ESLint** e **Prettier** configurados para garantir consistência e qualidade do código.

```bash
# Verificar problemas de lint
yarn lint

# Corrigir problemas automaticamente
yarn lint --fix
```

> Recomenda-se integrar o ESLint e o Prettier ao editor (ex: VSCode com as extensões `ESLint` e `Prettier - Code formatter`) para feedback em tempo real.

---

## Contribuindo

Contribuições são bem-vindas. Para mudanças significativas, abra uma *issue* primeiro para discutir o que deseja alterar.

1. Faça um **fork** do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/minha-feature`)
3. Faça commit das alterações (`git commit -m 'feat: adiciona minha feature'`)
4. Faça push para a branch (`git push origin feature/minha-feature`)
5. Abra um **Pull Request**

> Por favor, certifique-se de que os testes existentes continuam passando e adicione novos testes quando aplicável.

---

<p align="center">Desenvolvido por <a href="https://github.com/marcelofilipov">marcelofilipov</a></p>
