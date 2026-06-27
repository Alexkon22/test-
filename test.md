









  
#                   Название: DevShelf
---
 ###   Ваша техническая библиотека в одном клике:
 
---
О проекте:
DevShelf помогает разработчикам отслеживать прогресс чтения технической литературы. Мы создали его, потому что устали терять заметки и забывать, на какой странице остановились.

> Читай как никто 
                                              
  **Основная цель — объединить читающих айтишников и дать им удобный инструмент для конспектирования**
  
  ####  Основные возможности:
  
  1. Отслеживание прогресса чтения (в процентах)
  2. Создание заметок к каждой главе с поддержкой  кода
  3. Публичные полки для обмена подборками книг
  4. Статистика: сколько страниц прочитано за неделю.
  5. Тёмная тема для чтения ночью.
---
 #### Быстрый старт (инструкция):
 * Нужно клонировать репозиторий: git clone
   sh
   https://github.com/user/devshelf.git
   ```
 * установить зависимости
`sh
   npm install
    ```
* Запустить локально:
  `sh
  npm run dev.
  ```
* Открыть в браузере: ```http://localhost:3000.```

  ---
  ####                       Пример использования (блок с кодом на JavaScript):

 * Импортируем библиотеку:
    ```js
    import { bookshelf } from 'devshelf';
    ```
* Добавляем новую книгу:
  ```js
   bookshelf.add({ title: 'Чистый код', author: 'Роберт Мартин', pages: 464 });
  ```
* Отмечаем прогресс:
  ```js
  bookshelf.updateProgress('Чистый код', 150);
  ```
  ---
  ####             Технологический стек

|Frontend | Backend|Database|Dokumentation|
|---------|--------|---------| -------------------------|
|React, SCSS.| Node.js, Express.|PostgreSQL| storebook  
---

##  🔥 Как помочь проекту
<details>
<summary>👇(нажми, чтобы узнать что сделать)</summary>

 * **✔️Форкнуть репозиторий**
  * **🌿 ✔️Создать ветку**
`  it checut -b feature/amazing-idea`
  *  **✔️Закомитить измененения** 
  `git commit -m 'Добавил крутую фичу'`
  * **✔️Запушить** 
  `git push origin feature/amazing-idea` 
  * **✔️Открыть**   
  ` Pull Request`
</details>

---

## 📂 Структура проекта

<details>
<summary>📦 devshelf/ (нажми, чтобы развернуть)</summary>

```
📦 devshelf/
├── 📁 src/
│   ├── 📁 components/
│   │   ├── 📁 ui/            # Кнопки, модалки, инпуты
│   │   ├── 📁 books/         # Карточка книги, прогресс-бар
│   │   └── 📁 layout/        # Хедер, футер, сайдбар
│   ├── 📁 pages/
│   │   ├── 📄 Home.tsx       # Главная страница
│   │   ├── 📄 Shelf.tsx      # Полка с книгами
│   │   └── 📄 Stats.tsx      # Статистика чтения
│   ├── 📁 hooks/             # Кастомные хуки
│   ├── 📁 utils/
│   │   ├── 📄 formatters.ts  # Форматирование дат и чисел
│   │   └── 📄 validators.ts  # Валидация ISBN и email
│   └── 📄 App.tsx            # Корневой компонент
├── 📁 public/
│   └── 📄 favicon.ico
├── 📄 package.json
├── 📄 tsconfig.json
├── 📄 .env.example
└── 📄 README.md
```

</details>

---
## 💻 Примеры использования

<details>
<summary>JavaScript (нажми, чтобы показать код)</summary>

```javascript
import { bookshelf } from 'devshelf';

bookshelf.add({
  title: 'Чистый код',
  author: 'Роберт Мартин',
  pages: 464
});

bookshelf.updateProgress('Чистый код', 150);
```

</details>

<details>
<summary>Python (нажми, чтобы показать код)</summary>

```python
from devshelf import Bookshelf

shelf = Bookshelf()

shelf.add_book(
    title="Грокаем алгоритмы",
    author="Адитья Бхаргава",
    pages=288
)

shelf.update_progress("Грокаем алгоритмы", 144)
```

</details>

<details>
<summary>Bash (нажми, чтобы показать код)</summary>

```bash
# Установка
npm install -g devshelf-cli

# Добавление книги через терминал
devshelf add "Чистая архитектура" --author "Роберт Мартин" --pages 432

# Обновление прогресса
devshelf progress "Чистая архитектура" --page 200

</details>








