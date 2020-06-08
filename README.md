<div align="center">
    <img src="https://i.imgur.com/thB3TEi.png" width="300px"/>
</div>

<br />

<h2 align="center">
   NextLevelWeek 1.0
</h2>

<p align="center">
  <a href="#computer-project">Project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-built-with">Built with</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#information_source-how-to-run">How to run</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-license">License</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#mailbox_with_mail-get-in-touch">Get in touch</a>
  </p>

## :computer: Project 

 Ecoleta is an application that aims to connect people to point of collecting and recycle products.
 
## 🖼 Screenshot

<img src="https://i.imgur.com/sqxLEbx.jpg">

## :rocket: Built with

This project was developed with the following technologies:

-   [Node.js](https://nodejs.org/)
-   [ReactJS](https://reactjs.org/)
-   [React Native](https://facebook.github.io/react-native/)
-   [TypeScript](https://github.com/microsoft/TypeScript)
-   [TypeORM](https://typeorm.io/)
-   [Express](https://expressjs.com/)
-   [Context API](https://reactjs.org/docs/context.html)
-   [Styled-components](https://www.styled-components.com/)
-   [React Navigation](https://reactnavigation.org/)
-   [React-icons](https://react-icons.netlify.com/)
-   [Axios](https://github.com/axios/axios)
-   [React-toggle](https://github.com/aaronshaf/react-toggle)
-   [React-spring](https://www.react-spring.io/)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [VS Code](https://code.visualstudio.com/)


## :information_source: How to run

### Requirements

To run the application you will need:
* [Git](https://git-scm.com)
* [Node](https://nodejs.org/)
* [Yarn](https://yarnpkg.com/) 

I strongly recommend using [Docker](https://www.docker.com/) to run the databases.
<br>
If you decide to use docker, follow this steps to install and run the docker image.

```bash
# install Postgres image (if you don't specify an username it will be postgres by default)
$ docker run --name imagename -e POSTGRES_PASSWORD=yourPassword -p 5432:5432 -d postgres

# start Postgres
$ docker start imageName

```
### Backend
Now clone the repository and install the dependencies.
```bash
# to clone the repository
$ git clone https://github.com/StefanoSaffran/ecoleta.git

# go into the backend folder
$ cd ecoleta/backend

#install the backend dependencies
$ yarn

```
In order to connect to the database, you will need to enter the access informations into a ormconfig.json. You can find more about it [here](https://typeorm.io/#/using-ormconfig).

```bash
# run migrations
$ yarn typeorm migration:run

# run api
$ yarn dev:server
```

### Frontend

```bash
# in another tab of the terminal install the frontend dependencies and run it 
$ cd frontend
$ yarn
$ yarn start
```

### Mobile

The Application was developed using Expo. It is a free and open source toolchain built around React Native to facilitate the process of running and testing applications. [Click here](https://expo.io/learn) to get start with Expo.

```bash
# install the dependencies
cd mobile
yarn
```

In order to run the application on your device, you need to change the ip config.

[api.ts](https://github.com/adroaldopagliari/ecoleta/blob/master/mobile/src/services/api.ts)
```javascript
  baseURL: 'http://192.168.0.185:3333',
```
replace 192.168.0.185 with your machine's ip.

Now with everything on place, run the application.

```bash

# to run the app
yarn start

```
Expo will open a page in your browser, scan the QRcode on the page and wait for the app to load.

> The Application was developed and tested on Iphone 6s and Android Studio Emulator.

## :memo: License

This project is under the MIT license. See the [LICENSE](https://github.com/StefanoSaffran/ecoleta/blob/master/LICENSE) for more information

## :mailbox_with_mail: Get in touch!

<a href="https://www.linkedin.com/in/adroaldopagliari/" target="_blank" >
  <img alt="Linkedin - Adroaldo Pagliari" src="https://img.shields.io/badge/Linkedin--%23F8952D?style=social&logo=linkedin">
</a>&nbsp;&nbsp;&nbsp;
<a href="mailto:adroaldo@outlook.com" target="_blank" >
  <img alt="Email - Adroaldo Pagliari" src="https://img.shields.io/badge/Email--%23F8952D?style=social&logo=gmail">
</a> 

---

