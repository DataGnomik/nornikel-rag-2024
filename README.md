## Мультимодальная система RAG с использованием ColPali + Qwen-2-VL

Решение задания в рамках соревнования Норникеля.

Этот репозиторий содержит несколько ноутбуков, реализующих мультимодальную систему на базе **Retrieval-Augmented Generation (RAG)**. Система работает с векторными базами данных и интегрирует текст и изображения для генерации ответов. В частности, используется фреймворк [**byaldi**](https://github.com/AnswerDotAI/byaldi), а модель 🤗 [colpali-v1.2](https://huggingface.co/vidore/colpali-v1.2) предназначена для обработки мультимодальных запросов (текст и изображения). Для обработки текстового запроса с изображениями для инференса используется модель 🤗 [Vikhr-2-VL-2b-Instruct-experimental](https://huggingface.co/Vikhrmodels/Vikhr-2-VL-2b-Instruct-experimental).

Для успешной работы обязательно потребуются данные хакатона, скачать можно [здесь](https://drive.google.com/file/d/1bHGJGOnVtRYCl7LJ8eR7VGwKd6C7eMK6/view?usp=drive_link).

## Информация о ноутбуках

Существует две версии решения: 
- полная версия в одном ноутбуке (выполнение индексации документов + генерация ответов через VLM).
- [две части полной версии](https://github.com/metanovus/nornikel-rag-2024/tree/main/notebooks/for_testing) (Часть 1 - для создания векторной БД, часть 2 - для инференсов).

## Требования

Для работы с проектом вам потребуется установить следующие зависимости:

- Python 3.x
- PyTorch
- Hugging Face Transformers
- Byaldi (для работы с векторными базами)
- Pillow (для обработки изображений)
- NumPy, Pandas (для обработки данных)
- Jupyter Notebook (для демонстрации работы модели)
- другие зависимости, указанные в `requirements.txt`

## Установка

1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/metanovus/nornikel-rag-2024.git
   cd nornikel-rag-2024
   ```

2. Установите зависимости:
   ```bash
   pip install -r requirements.txt
   ```
