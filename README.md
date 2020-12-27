# Socket Chat - Client

Simple single page chat application - Client part.

For server part go to [socket chat server](https://github.com/IVIosi/socket-chat-server).

## How It Works
### Technologies And Libraries
App is powered by [React JS](http://reactjs.org/) and [socket.io](http://socket.io/).
- [Babel](https://github.com/babel/babel) for transcompiling code and backward compatibility.
- [Webpack](https://github.com/webpack/webpack) for bundling purposes.
- [Jest](https://github.com/facebook/jest) and [RTL (React Testing Library)](https://github.com/testing-library/react-testing-library) for testing.
- [TypeScript](https://www.typescriptlang.org/) for adding types.
- [Sass](https://sass-lang.com/) as a stylesheet language.
- [ESLint](https://eslint.org/), [Stylelint](https://stylelint.io/) and [Prettier](https://prettier.io/) for linting and code format.

TypeScript codes are compiled with Babel. All types are checked in pre-commit stage using [lint-staged](https://github.com/okonet/lint-staged) and [husky](https://github.com/typicode/husky).

Styles are normalized to work properly on different browsers.
Sass variables are used for theming. Some mixins also added for some repeated styles. PostCSS used for automated adding of vendor prefixes and polyfilling modern CSS.

## Get Started Immediately
**You’ll need to have Node 10.16.0 or later version on your local development machine.** You can use [nvm](https://github.com/creationix/nvm#installation) (macOS/Linux) or [nvm-windows](https://github.com/coreybutler/nvm-windows#node-version-manager-nvm-for-windows) to switch Node versions between different projects.

**For working properly this app needs [socket chat server](https://github.com/IVIosi/socket-chat-server) up and running.**

1. Clone project.
2. Run ```npm ci``` in project root directory to install dependencies.
3. Rename **.env.example** to **.env** 
4. Start project in developement mode using ```npm run dev```

## Commands

- Test will run with ```npm run test``` and ```npm run test:watch```

- Code linting with ```npm run lint:code``` and style linting with ```npm run lint:style```

- Building project and make it ready for deployment with ```npm run build```.

## Structure of App

```
socket-chat-client
├── README.md
├── public
│   └── index.html
└── src
    ├── __tests__
    ├── components
    ├── helpers (Reusable utilities and custom hooks)
    ├── static (Base styles, images, SVG icons sprite)
    ├── app.tsx
    ├── index.tsx
    ├── styles.scss
    └── globals.d.ts
```

## Features
### Mentiond On Homework File:
Messages:
- [x] The user's messages is on the right and other user's is on the left.
- [x] Input field with support of sending by *enter* or *ctrl+enter*.
- [x] Users can send images by providing URL.
- [x] Send message and send image buttons.
- [x] Send message and send image buttons.

Settings:
- [x] Modal for settings form.
- [x] All settings consumed and saved on LocalStorage.
- [x] Change user name field.
- [x] Change clock display format field.
- [x] Change send by *enter* or *ctrl+enter* format field.
- [x] Change clock display format field.
- [x] Reset all settings to their defaults.

Other Features:
- [x] Responsiveness.
- [x] Working on Chrome and Firefox latest versions.


### Added Features:

- [x] Avatar.
- [x] A11y.
- [x] Display user name.
- [x] disabling on server error.
- [x] Display user name.





