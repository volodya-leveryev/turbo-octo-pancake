# Компиляция Docker-образа в GitHub Actions

1. Создать по шаблону свой репозиторий
2. Склонировать его на локальный компьютер
3. Создать виртуальное окружение и активировать его
   ```
   python -m venv venv
   venv\scripts\activate.bat
   ```
4. Установить в виртуальное окружение пакеты
   ```
   pip install -r requirements.txt
   ```
5. Протестировать приложение локально
   ```
   pytest
   ```
6. Добавить Dockerfile.
   ```
   FROM
   WORKDIR???
   COPY
   RUN
   CMD
   ```
9. Добавить описание GitHub Actions для:
   * автоматизированного тестирования
   * сборки Docker-образа 
   * публикация Docker-образа в реестре GitHub Container Registry
   * Запуск Docker-контейнера по образу из реестра GitHub Container Registry

**Дополнительные ссылки:**

* [Deploying Flask with Gunicorn](https://flask.palletsprojects.com/en/3.0.x/deploying/gunicorn/)
* [Dockerfile reference](https://docs.docker.com/engine/reference/builder/)
* [Описание Docker-образа для Python](https://hub.docker.com/_/python)
* [GitHub Actions Contexts](https://docs.github.com/en/actions/learn-github-actions/contexts)
* [GitHub Actions Checkout](https://github.com/actions/checkout)
* [GitHub Actions Setup Python](https://github.com/actions/setup-python)
* [GitHub Actions Build Docker image](https://github.com/docker/build-push-action)
