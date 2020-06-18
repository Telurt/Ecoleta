<h1 align=center>
<img src="https://user-images.githubusercontent.com/38081852/83580830-6f63e200-a513-11ea-9a27-0a109ec1e4d0.png" />
</h1>

<div align="center">

<a href="https://rocketseat.com.br">
<img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%237519C1">
</a>

</div>

<h3 align="center">

♻️ Ecoleta é um projeto **Open Source** desenvolvido na semana **Next Level Week (1.0)** da **[Rocketseat][rocketseat_site]** utilizando as tecnologias **_TypeScript, Node, React e React Native_**.

</h3>

![Banner](https://user-images.githubusercontent.com/38081852/84095189-04178580-a9d5-11ea-9496-9ec6f6a282e5.png)

## **:rocket: OBJETIVO**

O projeto tem como finalidade **estabelecer uma conexão** entre **empresas e/ou entidades que coletam resíduos** (orgânicos e inorgânicos) **às pessoas e/ou entidades que necessitam constantemente descartar esses resíduos**. Solucionando um grande problema recorrente que é o **descarte inadequado do lixo**, facilitando o processo de recliclagem e reutilização.

<!--
  ...
  Local Reservado para o GIF do projeto rodando.
  ...
-->

## **:computer: TECNOLOGIAS**

#### **Website** ([React] + [TypeScript])

- **[React Router Dom]**
- **[React Icons]**
- **[Axios]**
- **[Leaflet]**
- **[React Leaflet]**
- **[React Dropzone]**

\* Veja o arquivo <kbd>[package.json](./sources/website/package.json)</kbd>

#### **Server** ([NodeJS] + [TypeScript])

- **[Express]**
- **[CORS]**
- **[KnexJS]**
- **[SQLite]**
- **[ts-node]**
- **[dotENV]**
- **[Multer]**
- **[Celebrate]**
- **[Joi]**

\* Veja o arquivo <kbd>[package.json](./sources/server/package.json)</kbd>

#### **Mobile** ([React Native] + [TypeScript])

- **[Expo]**
- **[Expo Google Fonts]**
- **[React Navigation]**
- **[React Native Maps]**
- **[Expo Constants]**
- **[React Native SVG]**
- **[Axios]**
- **[Expo Location]**
- **[Expo Mail Composer]**

\* Veja o arquivo <kbd>[package.json](./sources/mobile/package.json)</kbd>


## **:wine_glass: COMO UTILIZAR**

### Configurações Iniciais

Primeiro, você precisa ter o <kbd>[NodeJS](https://nodejs.org/en/download/)</kbd> instalado na sua máquina.

Se você estiver utilizando o **Linux**, você pode optar por instalar o **Node** através do gerênciador de versões <kbd>[asdf]</kbd> para facilitar o processo de mudança da versão do **Node**, quando for necessário.

Você pode optar também por utilizar o **yarn** no lugar do **npm**. Você pode instalar clicando nesse <kbd>[link][yarn]</kbd>, ou através do <kbd>[asdf]</kbd>.

Após ter o **Node** instalado, instale as dependências do **React e React Native (Expo)** de forma global, utilizando os comandos:

```sh
# React:
$ npm install create-react-app -g

# Expo (React Native):
$ npm install -g expo-cli
```

Você precisa renomear o arquivo `.env-example` para `.env` e inserir as informações que condizem com o seu **host**:

```sh
$ mv .env-example .env
```

Instale as dependências contidas nos arquivos `package.json` que se encontram na raíz do repositório (para o gerenciamento de commits), no diretório do **server**, no diretório do **website** e no diretório **mobile**. Para instalar as dependências, basta abrir o terminal no diretório e digitar o comando:

```sh
$ npm install

# ou
$ yarn
```

Exemplos:

```sh
# Instalando as dependências do commitlint:
$ cd ./ecoleta
$ npm install

# Instalando as dependências do server:
$ cd ./sources/server
$ npm install

# Instalando as dependências do website:
$ cd ./sources/website
$ npm install

# Instalando as dependências do mobile:
$ cd ./sources/mobile
$ npm install
```

Veja os arquivos **`package.json`** do <kbd>[commitlint](./package.json)</kbd>, <kbd>[server](./sources/server/package.json)</kbd>, <kbd>[website](./sources/website/package.json)</kbd> e <kbd>[mobile](./sources/mobile/package.json)</kbd>.

### Utilizando o Server

```sh
# Abrindo o terminal no diretório do servidor:
$ cd ./sources/server

# Executando a aplicação em modo de desenvolvimento:
$ npm run dev

# Instanciando o banco de dados:
$ npm run knex:migrate

# Povoando o banco de dados (seeds):
$ npm run knex:seed
```

> Veja a parte de **scripts {}** do arquivo <kbd>[package.json](./sources/server/package.json)</kbd> para saber quais scripts estão disponíveis.

### Utilizando o Website

```sh
# Abrindo o terminal no diretório do website:
$ cd ./sources/website

# Executando o website no modo de desenvolvimento:
$ npm run start
```

> Se o browser não abrir automaticamente, acesse: http://localhost:3000.

### Utilizando o Mobile

Instale o aplicativo <kbd>[Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en)</kbd> no seu smartphone.

```sh
# Abrindo o terminal no diretório do mobile:
$ cd ./sources/mobile

# Executando o mobile no modo de desenvolvimento:
$ npm run start
```

Agora, abra o aplicativo do expo e no modo **LAN** faça o scan do QRCode.

> Se tiver algum problema para executar o aplicativo nesse modo, tente desabilitar o firewall da sua máquina.

Se tiver algum problema com as fontes, utilize o comando:

```sh
$ expo install expo-font @expo-google-fonts/ubuntu @expo-google-fonts/roboto
```

**\* Lembre de inserir no arquivo `.env` o IP exato que foi gerado pelo seu mobile após utilizar o comando `npm run start`.**

## **:octocat: COMO CONTRIBUIR**

- Verifique as **[Issues](https://github.com/x0n4d0/ecoleta/projects/1)** que estão abertas e se já não existe alguma com a sua feature;
- Abra uma **Issue** com o nome e descrição da sua feature e assine com o seu usuário informando que irá fazê-la;
- Faça um **[fork](https://help.github.com/pt/github/getting-started-with-github/fork-a-repo)** do repositório;
- Entre no sua página do GitHub e faça um **clone** do seu **fork**;
- Crie uma _branch_ com o nome da sua feature: `git chechout -b feat/minhaFeature`;
- Faça as alterações necessárias no código ou na documentação;
- Instale as dependências do _commitlint_ na raíz do projeto para a verificação dos commits: `npm install` ou `yarn`;
- Faça o _commit_ das suas alterações seguindo as [convenções de commit](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/), adicione na descrição o id da sua Issue em parênteses e lembre de fechar a sua Issue com o id no rodapé do commit:

```
  <tipo>(escopo opcional): <descrição> (#x)

  [corpo do commit]

  Close #x
```

Exemplo:

```sh
  feat: adicionado componente para tal coisa (#52)

  Foi adicionado um componente para tal coisa com o objetivo de melhorar tal coisa, deixando o projeto de tal maneira.

  Close #52
```

- Faça um _push_ para a sua _branch_: `git push origin feat/minhaFeature`;
- Agora é só abrir um _pull request_ no repositório que você fez o _fork_ e assim que acontecer o _merge_ sua Issue será fechada e suas alterações irão fazer parte do projeto;
- Depois que o _merge_ da sua pull request for feito, você pode deletar a sua _branch_.


## **:page_with_curl: LICENÇA**

Esse repositório está licenciado pela **MIT LICENSE**. Para mais informações detalhadas, leia o arquivo [LICENSE](./LICENSE) contido nesse repositório.

<h2 align="center"> Desenvolvido por <a href="https://www.linkedin.com/in/telsonurtiga/">Telson Urtiga</a></h2>
