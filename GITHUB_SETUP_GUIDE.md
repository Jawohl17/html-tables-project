# 📘 Інструкція по налаштуванню GitHub

## ✅ Виконано

- ✓ Git репозиторій ініціалізовано (`git init`)
- ✓ Створено **6 комітів** (вимагалось мінімум 5)
- ✓ Додано файл README.md з описом проєкту
- ✓ Створено головну сторінку index.html для GitHub Pages

## 📋 Наступні кроки

### Крок 1: Створення віддаленого репозиторію на GitHub

1. Перейдіть на **https://github.com**
2. Натисніть кнопку **"+"** у правому верхньому куті → **"New repository"**
3. Заповніть форму:
   - **Repository name**: `html-tables-project` (або інше ім'я на ваш вибір)
   - **Description**: "HTML Tables Project - collection of table examples"
   - **Public** (обов'язково для GitHub Pages)
   - **НЕ вмикайте** "Initialize this repository with a README" (у нас вже є README.md)
4. Натисніть **"Create repository"**

### Крок 2: Підключення віддаленого репозиторію

Після створення репозиторію GitHub покаже вам команди. Використайте такі команди в PowerShell:

```powershell
# Замініть [ваш-юзернейм] на ваше ім'я користувача GitHub
git remote add origin https://github.com/[ваш-юзернейм]/html-tables-project.git

# Перевірте, що remote додано успішно
git remote -v
```

**Приклад:**
```powershell
git remote add origin https://github.com/student123/html-tables-project.git
```

### Крок 3: Запуш локального репозиторію на GitHub

Виконайте команду для відправки коду на GitHub:

```powershell
# Для нових версій Git (main гілка)
git branch -M main
git push -u origin main

# АБО для старих версій Git (master гілка)
git push -u origin master
```

**Примітка:** Якщо у вас з'явиться вікно авторизації, введіть свої облікові дані GitHub.

### Крок 4: Активація GitHub Pages

1. Перейдіть на сторінку вашого репозиторію на GitHub
2. Клікніть на **"Settings"** (Налаштування)
3. У лівому меню знайдіть розділ **"Pages"**
4. У секції **"Source"** виберіть:
   - **Branch**: `main` (або `master`)
   - **Folder**: `/root` (або `/(root)`)
5. Натисніть **"Save"**
6. Зачекайте 1-2 хвилини - GitHub згенерує сторінку

### Крок 5: Отримання посилань

**Посилання на репозиторій:**
```
https://github.com/[ваш-юзернейм]/html-tables-project
```

**Посилання на GitHub Pages:**
```
https://[ваш-юзернейм].github.io/html-tables-project/
```

**Приклад:**
- Репозиторій: `https://github.com/student123/html-tables-project`
- GitHub Pages: `https://student123.github.io/html-tables-project/`

### Крок 6: Перевірка роботи сторінки

1. Відкрийте посилання GitHub Pages у браузері
2. Перевірте, що всі сторінки відображаються коректно:
   - `index.html` - головна сторінка
   - `table1.html` - таблиця з різними висотами
   - `table2.html` - вкладена таблиця
   - `table3.html` - таблиця Мондріана

### Крок 7: Використання Issues

1. На сторінці репозиторію перейдіть у вкладку **"Issues"**
2. Натисніть **"New issue"**
3. Створіть кілька Issues для відстеження задач, наприклад:

**Issue 1: Додати навігаційне меню**
```
Title: Add navigation menu
Description: Add a navigation menu to easily switch between different table examples
Labels: enhancement
```

**Issue 2: Покращити адаптивність**
```
Title: Improve mobile responsiveness
Description: Make tables more responsive on mobile devices
Labels: enhancement
```

**Issue 3: Додати більше прикладів**
```
Title: Add more table examples
Description: Create additional examples with complex table structures
Labels: feature
```

## 🎯 Що потрібно надіслати викладачу

1. **Посилання на репозиторій GitHub:**
   `https://github.com/[ваш-юзернейм]/html-tables-project`

2. **Посилання на GitHub Pages:**
   `https://[ваш-юзернейм].github.io/html-tables-project/`

## 💡 Додаткові команди Git

```powershell
# Переглянути статус репозиторію
git status

# Переглянути історію комітів
git log --oneline

# Переглянути віддалені репозиторії
git remote -v

# Переглянути всі гілки
git branch -a
```

## 🔧 Вирішення можливих проблем

### Проблема: GitHub Pages не працює

**Рішення:**
1. Перевірте, що репозиторій публічний (Public)
2. Переконайтеся, що `index.html` знаходиться в кореневій папці
3. Зачекайте 5-10 хвилин після активації GitHub Pages
4. Перевірте вкладку "Actions" - там можна побачити процес розгортання

### Проблема: Помилка при push

**Рішення:**
```powershell
# Якщо віддалений репозиторій вже містить файли
git pull origin main --allow-unrelated-histories
git push -u origin main
```

### Проблема: Неправильний remote

**Рішення:**
```powershell
# Видалити старий remote
git remote remove origin

# Додати новий remote
git remote add origin https://github.com/[ваш-юзернейм]/[назва-репозиторію].git
```

## 📚 Корисні посилання

- [GitHub Docs - Creating a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Issues Guide](https://docs.github.com/en/issues)

---

**Удачі з виконанням практичної роботи! 🚀**

