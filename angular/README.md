Установка среды разработки под Ангуляр 2 (под c9.io)
=========================================

Для начала установить последнюю версию Node.js.

Затем следует установить глобально [командную строку Ангуляра](https://www.npmjs.com/package/@angular/cli):

```bash
npm i -g @angular/cli
```

Далее создаем папку под проект и в ней запускаем команду:

```bash
ng new --style=scss --skip-git --routing --skip-install <папка проекта>
```

Опция `--skip-install` позволяет процесс установки NPM-модулей.
Без этой опции в конце создания проекта будет запущена команда `npm i`.

Вы можете добавить опцию `--routing` в команду `ng new` чтобы появился 
файл `app-routing.module.ts` где будут хранится отдельно маршрутизация 
вашего проекта.

Для c9.io файл package.json подправляем следующим образом:

```json
"start": "ng serve --host 0.0.0.0",
```

Обновление командной строки Ангуляра
--------------

```bash
npm uninstall -g @angular/cli
npm cache clean
npm install -g @angular/cli@latest
```

Подробнее на  
https://github.com/angular/angular-cli  
https://angular.io/docs/ts/latest/cli-quickstart.html  
