# CRA setup

Данная директория существует для хранения файлов, которые мы будем использовать, когда работаем через create-react-app.
Разумеется, учитывая что это cra - поддерживается вообще все, все быстро и оптимизировано.
На старте, получается react приложение, с настроенной связкой линтера и форматтера. Далее уже все зависит от проекта.

## Алгоритм раскатки окружения

- npx create-react-app name-of-project
- cd name-of-project
- code .
- open a folder in Finder and delete hidden .git folder
- clear env, delete files, comments, change html titles&stuff
- change index.css and fill it w/ nearby index.css file in this repo
- change file extensions from .js to .jsx when its needed
- npm init
- clear eslint related stuff from package.json
- npm init @eslint/config
- change created eslint cofig w/ urs
- add this two to scripts in package.json

```
    "lint": "eslint --ext .js,.jsx src/",
	"lint-fix": "eslint --fix --ext .js,.jsx src/"
```

- npm install prettier eslint-config-prettier eslint-plugin-prettier --save-dev
- create .prettierrc.json and fill it w/ ur settings
- save it all, to check if prettier works
- check if eslint is in sync w/ create-react-app (i recommend turn on comments errors and check it)
- happy coding !

_Something to mention_
prettier uses vscode extenstion, and change everything on every cmd+s, cuz of vscode settings we made. So yeah, there is a few little sets on vscode - just fyi, in case someday u'll reinstall vscode

## in case u using tailwind

- open installation docs and go w/ cra docs
- after u'll set up things w/ docs run - npm install -D prettier prettier-plugin-tailwindcss
- also gotta mention dat we have installed and setted vscode tailwind extension, in case vscode reinstallation - tailwind docs and extensions itself docs will help u setup it
- u good to go
