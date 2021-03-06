Старт проекта на TypeScript
==============================




В директории проекта (директория должна быть пустой или с .idea):

```bash
npx create-react-app .
npm install --save typescript @types/node @types/react @types/react-dom @types/jest
```

Переименовать файлы:

```
App.test.js -> App.test.tsx
App.js -> App.tsx
index.js -> index.tsx
```

Сделать первый запуск:

```bash
npm start
```

Внимание, после первого запуска будут автоматически созданы два файла:

```
src/react-app-env.d.ts
tsconfig.json
```


.gitignore
----------

```json
node_modules
npm-debug.log
/.pnp
.pnp.js

# testing
/coverage

# production
/build
/target

# misc
/.idea
.DS_Store
.env.local
.env.development.local
.env.test.local
.env.production.local

npm-debug.log*
yarn-debug.log*
yarn-error.log*
```



Файл tslint.json
----------------

```json
{
  "extends": ["tslint:recommended", "tslint-react", "tslint-config-prettier"],
  "rules": {
    "no-console": false,
    "ordered-imports": false,
    "object-literal-sort-keys": false,
    "no-empty": [true, "allow-empty-functions"]
  },
  "linterOptions": {
    "exclude": [
      "config/**/*.js",
      "node_modules/**/*.ts"
    ]
  }
}
```

Файл tsconfig.json
------------------

```json
{
  "compilerOptions": {

    "lib": ["es6", "dom", "es2017"],
    "typeRoots": ["node_modules/@types"],

    "target": "es5",
    "allowJs": true,
    "skipLibCheck": false,
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true,
    "strict": true,
    "forceConsistentCasingInFileNames": true,
    "module": "esnext",
    "moduleResolution": "node",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "noEmit": true,
    "jsx": "preserve"
  },
  "include": [
    "src"
  ]
}
```

rewired
-------

https://github.com/timarney/react-app-rewired
