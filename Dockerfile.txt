# Указываем базовый образ с Python
FROM python:3.9-slim

# Создаем рабочую директорию
WORKDIR /app

# Копируем наш файл main.py внутрь контейнера
COPY main.py .

# Устанавливаем зависимости (если нужны)
# RUN pip install -r requirements.txt

# Команда, которая будет выполняться при запуске контейнера
CMD ["python", "main.py"]
