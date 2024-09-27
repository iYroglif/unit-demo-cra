test4
### [commitlint](.github/workflows/commitlint.yml)

Проверяет соответствия сообщений о коммитах формату conventional commits

### [pull-request](.github/workflows/pull-request.yml)

Запускает линтер и автотесты

### [release](.github/workflows/release.yml)

Создает релизную ветку, создает запись в реестре релизов (issues) со всей важной информацией, запускает проверки аналогичные pull-request и если они прошли выкладывает приложение на github-pages и закрывает issue

## В этом репозитории находится пример приложения с тестами:

-   [e2e тесты](e2e/example.spec.ts)
-   [unit тесты](src/example.test.tsx)

Для запуска примеров необходимо установить [NodeJS](https://nodejs.org/en/download/) 16 или выше.

Как запустить:

```sh
# установить зависимости
npm ci

# запустить приложение
npm start
```

Как запустить e2e тесты:

```sh
# скачать браузеры
npx playwright install

# запустить тесты
npm run e2e
```

Как запустить модульные тесты:

```sh
npm test
```
