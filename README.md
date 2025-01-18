# 24 Photo Filter

## Описание
Этот проект предназначен для применения фильтров к изображениям с использованием Python. Он включает в себя инструменты для обработки изображений и их отображения. Основной файл проекта: `my-filter.ipynb`.

## Структура проекта
```
24_photo_filter
├── .ipynb_checkpoints/       # Системные файлы Jupyter Notebook
├── linux-venvs/             # Виртуальная среда Python
│   ├── bin/                 # Исполняемые файлы виртуальной среды
│   ├── lib/                 # Зависимости и библиотеки
│   └── ...
├── photo/                   # Папка с изображениями
│   ├── elephants.jpg        # Пример изображения
│   ├── procyon.jpg          # Пример изображения
├── .gitignore               # Список игнорируемых файлов
├── LICENSE                  # Лицензия проекта
└── my-filter.ipynb          # Основной Jupyter Notebook
```

## Установка

1. **Склонируйте репозиторий:**
   ```bash
   git clone git@github.com:pekarskii/24_photo_filter.git
   cd 24_photo_filter
   ```

2. **Создайте виртуальную среду:**
   ```bash
   python3 -m venv linux-venvs
   ```

3. **Активируйте виртуальную среду:**
   - Для Linux/MacOS:
     ```bash
     source linux-venvs/bin/activate
     ```
   - Для Windows:
     ```bash
     linux-venvs\Scripts\activate
     ```

4. **Установите зависимости:**
   ```bash
   pip install -r requirements.txt
   ```

## Использование

1. Добавьте ваши изображения в папку `photo`.
2. Откройте `my-filter.ipynb` с помощью Jupyter Notebook.
3. Выполните ячейки кода, чтобы применить фильтры к изображениям.

## Пример использования
Файл `photo/elephants.jpg` используется для тестирования фильтров. В Jupyter Notebook вы можете загрузить это изображение и применить к нему фильтры.

Пример кода для загрузки изображения:
```python
from PIL import Image

# Загрузка изображения
path = 'photo/elephants.jpg'
image = Image.open(path)
image.show()
```

## Лицензия
Этот проект распространяется под лицензией [MIT](LICENSE).

## Вклад в проект
Если вы хотите внести свой вклад:
1. Форкните репозиторий.
2. Создайте новую ветку: `git checkout -b feature-branch-name`
3. Внесите изменения и зафиксируйте их: `git commit -m 'Описание изменений'`
4. Отправьте изменения: `git push origin feature-branch-name`
5. Создайте Pull Request.
