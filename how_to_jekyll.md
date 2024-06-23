---
layout: default
---

## Инструкция по установке Jekyll и настройке локального тестирования

Этот сайт документации работает на Jekyll — фреймворке для генерации статических сайтов на языке Ruby. Для удобного обновления и тестирования сайта вам нужно установить ряд инструментов и настроить окружение. Следуйте инструкциям ниже:


### 1. Установка Ruby и инструментов Jekyll

1. **Установите Ruby**:

   - Перейдите на [официальный сайт RubyInstaller](https://rubyinstaller.org/).
   - Скачайте и установите последнюю версию Ruby с DevKit для вашей операционной системы.
   - Во время установки убедитесь, что выбрана опция «Add Ruby to PATH».

2. **Установите Jekyll**:

   - Откройте терминал (Command Prompt или PowerShell в Windows, Terminal в macOS/Linux).

   - Убедитесь, что Ruby и Gem установлены правильно, выполнив команду `ruby -v` и `gem -v`.

   - Установите Jekyll и Bundler, выполнив команду:

     ```sh
     gem install jekyll
     ```

### 2. Клонирование репозитория

1. **Сделайте Fork репозитория**:

   - Перейдите на страницу репозитория на GitHub.
   - Нажмите кнопку «Fork» в правом верхнем углу, чтобы создать копию репозитория в вашем аккаунте.

2. **Клонируйте репозиторий на локальную машину**:

   - Скопируйте URL вашей новой форкнутой версии репозитория.

   - В терминале выполните команду для клонирования:

     ```sh
     git clone 'URL_вашего_репозитория'
     ```

   - Замените `'URL_вашего_репозитория'` на фактический URL вашего форка.

### 3. Запуск локального сервера

1. **Перейдите в директорию клонированного репозитория**:

   - Используйте команду:

     ```sh
     cd имя_папки_репозитория
     ```

   - Замените `имя_папки_репозитория` на название папки, куда был клонирован репозиторий.

2. **Запустите локальный сервер Jekyll**:

   - Выполните команду:

     ```sh
     jekyll serve
     ```

   - Локальный сервер будет запущен, и сайт будет доступен по умолчанию по адресу `http://localhost:4000`.

3. **Откройте сайт в браузере**:

   - Перейдите в браузере по адресу `http://localhost:4000`, чтобы просмотреть и тестировать ваш сайт.


![local_server](https://github.com/pedohorse/cg-community-hub/assets/47521478/3ccfdbee-5556-49a1-b8fa-d3ce14db69b2)

### 4. Устранение возможных ошибок

1. **Проверка версии Ruby и Bundler**:
   - Убедитесь, что используете совместимые версии Ruby и Bundler, так как некоторые версии могут конфликтовать с Jekyll.
2. **Проверка пути и окружения**:
   - Убедитесь, что переменная PATH вашего окружения содержит путь к установленному Ruby и Gem.

### 5. Завершение работы

1. **Остановите сервер**:

   - Для остановки локального сервера нажмите `Ctrl + C` в терминале.

2. **Внесите изменения и сохраните**:

   - Внесите нужные изменения в локально клонированный репозиторий. Эти изменения можно тестировать на локальном сервере.

3. **Запушьте изменения в ваш Fork**:

   - Используйте команды `git` для коммита и пуша ваших изменений обратно в ваш форкнутый репозиторий:

     ```sh
     git add .
     git commit -m "Ваше сообщение о коммите"
     git push origin ветка
     ```

   - Замените `ветка` на нужную вам ветку, например, `main` или `master`.

Теперь ваш локальный сервер настроен, и вы можете тестировать и вносить изменения в документацию сайта с помощью Jekyll.
