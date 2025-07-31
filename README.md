# Login com Github

## 📝 Descrição

O **ignews-login** é uma aplicação web desenvolvida como projeto de algumas aulas da Rocketseat, utilizando **Next.js** e **React**, que implementa autenticação social utilizando o **NextAuth.js** (login com GitHub). O projeto utiliza **TypeScript** para tipagem estática, **Sass** para estilização e integra também a biblioteca **Stripe** para futuras funcionalidades de pagamentos.

Atualmente, o app permite ao usuário autenticar-se com sua conta do GitHub, exibindo seu nome e um botão para logout. O layout é responsivo e utiliza ícones do pacote **react-icons**.

---

## 💻 Tecnologias Utilizadas

- **Next.js** (v15.3.5)
- **React** (v19.1.0)
- **TypeScript**
- **NextAuth.js** (v4.24.11)
- **Sass**
- **Stripe** (biblioteca instalada, integração futura)
- **React Icons**

---

## ⚙️ Como rodar o projeto

### 1. Pré-requisitos 

- **Node.js** (recomenda-se versão 18 ou superior)
- **npm** ou **yarn**

### 2. Instalação 

Clone o repositório e acesse a pasta do projeto:

```bash
git clone <url-do-repositorio>
cd ignews
```

Instale as dependências:

```bash
npm install
# ou
yarn install
```

### 3. Configuração das variáveis de ambiente 🔨

Crie um arquivo `.env.local` na raiz do projeto com as seguintes variáveis (exemplo para autenticação GitHub):

```
GITHUB_ID=seu_client_id_github
GITHUB_SECRET=seu_client_secret_github
NEXTAUTH_URL=http://localhost:3000
```

> Você pode obter o `GITHUB_ID` e `GITHUB_SECRET` criando um OAuth App em [GitHub Developer Settings](https://github.com/settings/developers).

### 4. Rodando o projeto

Para iniciar o servidor de desenvolvimento:

```bash
npm run dev
# ou
yarn dev
```

Acesse [http://localhost:3000](http://localhost:3000) no navegador.

---

## Estrutura do Projeto 🪜

- `src/pages/_app.tsx`: Configuração global do app, incluindo o provider do NextAuth.
- `src/components/Header`: Cabeçalho da aplicação.
- `src/components/SignInButton`: Botão de login/logout com GitHub.
- `src/styles/global.scss`: Estilos globais.

---

## O que o app faz até o momento

- Permite login com GitHub usando NextAuth.js.
- Exibe o nome do usuário autenticado e botão de logout.
- Layout responsivo e estilizado com Sass.
- Estrutura pronta para integração com Stripe.

---

## Observações 📃

- O projeto está em desenvolvimento e novas funcionalidades serão adicionadas.
- Para dúvidas sobre configuração do NextAuth.js, consulte a [documentação oficial](https://next-auth.js.org/getting-started/introduction).

---