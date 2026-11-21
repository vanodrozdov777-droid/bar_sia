BAR DESK — ГОТОВЫЙ ПРОЕКТ ДЛЯ GITHUB + ANDROID APK

ВАЖНО: загружайте СОДЕРЖИМОЕ этой папки в КОРЕНЬ существующего репозитория bar_sia.
Не загружайте ZIP как один файл и не создавайте внутри репозитория папку BAR-DESK-READY.

КАК ЗАГРУЗИТЬ:
1. Распакуйте ZIP на компьютере.
2. Откройте GitHub -> репозиторий bar_sia -> вкладка Code.
3. Нажмите Add file -> Upload files.
4. Откройте распакованную папку BAR-DESK-READY и выделите ВСЁ её содержимое, включая скрытую папку .github.
5. Перетащите всё в окно Upload files. Разрешите объединение/замену файлов, если GitHub спросит.
6. Нажмите Commit changes.

В корне репозитория должны лежать:
- index.html
- settings.gradle
- build.gradle
- gradle.properties
- папка app/
- папка .github/workflows/ с build-apk.yml и main.yml

Затем:
1. Откройте Actions.
2. Выберите Build BAR DESK APK.
3. Нажмите Run workflow -> Run workflow (если автоматическая сборка ещё не запустилась).
4. Дождитесь зелёной галочки.
5. Откройте успешный запуск и скачайте Artifact BAR-DESK-APK.
6. В ZIP-артефакте находится app-debug.apk.

ПРИМЕЧАНИЯ:
- APK собирается в GitHub Actions; Android Studio на компьютере не нужна.
- Это debug APK для установки и проверки, не релиз Google Play.
- Приложение открывает встроенную копию index.html.
- Данные, сохранённые в приложении, локальны для устройства.
- В архиве main.yml заменяет ранее созданный пустой workflow, чтобы новые запуски этого workflow завершались успешно.
