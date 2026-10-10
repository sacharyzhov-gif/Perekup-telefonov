СБОРКА APK С ТЕЛЕФОНА

1. Распакуй архив на Android.
2. Создай репозиторий на https://github.com/ (New repository).
3. Загрузи содержимое папки проекта в корень репозитория, сохранив структуру:
   - папка www с index.html
   - папка .github/workflows с android.yml
   - package.json
   - capacitor.config.json
4. Открой вкладку Actions в репозитории. Если GitHub попросит разрешить Actions — разреши.
5. Выбери workflow "Build Android APK" и нажми Run workflow (или сделай commit, чтобы запустить сборку автоматически).
6. Дождись зелёной галочки, открой запуск workflow, внизу раздел Artifacts и скачай simulator-perekupa-debug-apk.
7. Распакуй скачанный artifact ZIP и нажми на app-debug.apk. Разреши установку из этого источника, если Android спросит.

Важно:
- Нужен аккаунт GitHub и интернет.
- APK будет debug-сборкой для установки на своё устройство, не для публикации в Google Play.
- Если GitHub через браузер не даёт загрузить скрытую папку .github, включи в браузере «Версия для ПК» либо загрузи файлы через git-клиент/терминал. Workflow-файл должен лежать именно по пути .github/workflows/android.yml.
- Это стартовая версия игры, сохранение хранится локально в приложении.
