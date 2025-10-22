# 🚀 Як створити репозиторій на GitHub - Покрокова інструкція

## 📝 Варіант 1: Через веб-сайт GitHub (5 хвилин)

### Крок 1: Відкрийте GitHub
1. Перейдіть на **https://github.com**
2. Увійдіть у свій акаунт (якщо ще не увійшли)

### Крок 2: Створіть новий репозиторій
1. У правому верхньому куті натисніть кнопку **"+"**
2. Виберіть **"New repository"**

   ```
   [+] ▼
   ├─ New repository    ← НАТИСНІТЬ ЦЕ
   ├─ Import repository
   ├─ New gist
   └─ New organization
   ```

### Крок 3: Заповніть форму

```
Repository name*     [html-tables-project]
                     ↑ Введіть це ім'я

Description          [HTML Tables Project - collection of table examples]
(optional)           ↑ Введіть цей опис

● Public             ← ОБОВ'ЯЗКОВО виберіть Public (для GitHub Pages)
○ Private

☐ Add a README file              ← НЕ вмикайте (у вас вже є)
☐ Add .gitignore
☐ Choose a license

         [Create repository]     ← Натисніть цю кнопку
```

### Крок 4: Скопіюйте URL репозиторію

Після створення GitHub покаже вам сторінку. Знайдіть URL, він виглядає так:
```
https://github.com/[ваше-ім'я]/html-tables-project.git
```

**Приклад:** `https://github.com/ivanov123/html-tables-project.git`

📋 **Скопіюйте цей URL!** (натисніть на кнопку 📋 поруч з URL)

---

## 💻 Крок 5: Підключіть локальний репозиторій до GitHub

Тепер поверніться до PowerShell і виконайте:

```powershell
# Підключіть віддалений репозиторій (вставте ваш URL)
git remote add origin https://github.com/[ваше-ім'я]/html-tables-project.git

# Перевірте підключення
git remote -v

# Перейменуйте гілку на main
git branch -M main

# Запуште код на GitHub
git push -u origin main
```

### 📋 Готова команда для копіювання:

**⚠️ ВАЖЛИВО: Замініть `[ваше-ім'я]` на ваш GitHub username!**

Скопіюйте і вставте в PowerShell (після заміни username):
```powershell
git remote add origin https://github.com/[ваше-ім'я]/html-tables-project.git && git branch -M main && git push -u origin main
```

**Для PowerShell (окремі команди):**
```powershell
git remote add origin https://github.com/[ваше-ім'я]/html-tables-project.git
git branch -M main
git push -u origin main
```

---

## ⚠️ Можливі проблеми та рішення

### Проблема 1: Помилка авторизації

Якщо з'явиться вікно авторизації:
1. Введіть ваш GitHub username
2. Введіть ваш GitHub пароль або **Personal Access Token**

**Якщо потрібен Personal Access Token:**
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token → Введіть назву → Виберіть `repo` → Generate
3. Скопіюйте токен і використайте замість пароля

### Проблема 2: Remote вже існує

Якщо бачите помилку `remote origin already exists`:
```powershell
git remote remove origin
git remote add origin https://github.com/[ваше-ім'я]/html-tables-project.git
```

### Проблема 3: Не можу запушити

```powershell
# Спробуйте спочатку pull
git pull origin main --allow-unrelated-histories

# Потім push
git push -u origin main
```

---

## 🎉 Крок 6: Активуйте GitHub Pages

1. На сторінці вашого репозиторію на GitHub
2. Клікніть **Settings** (вгорі)
3. У лівому меню знайдіть **Pages**
4. У розділі **Source**:
   - **Branch**: `main`
   - **Folder**: `/(root)`
5. Натисніть **Save**
6. ⏳ Зачекайте 2-3 хвилини

GitHub покаже вам посилання:
```
✅ Your site is live at https://[ваше-ім'я].github.io/html-tables-project/
```

---

## 📦 Що здати викладачу

**1. Посилання на репозиторій:**
```
https://github.com/[ваше-ім'я]/html-tables-project
```

**2. Посилання на GitHub Pages:**
```
https://[ваше-ім'я].github.io/html-tables-project/
```

---

## 🎯 Крок 7: Створіть Issues (додаткове завдання)

1. На GitHub відкрийте вкладку **Issues**
2. Натисніть **New issue**

**Issue 1:**
```
Title: Add navigation menu
Description: Create a navigation menu to easily switch between different table examples
Labels: enhancement
```

**Issue 2:**
```
Title: Improve mobile responsiveness  
Description: Make tables more responsive on mobile devices
Labels: enhancement
```

**Issue 3:**
```
Title: Add more table examples
Description: Create additional examples with complex table structures
Labels: feature
```

---

## ✅ Чеклист виконання

- [ ] Створено репозиторій на GitHub
- [ ] Виконано `git remote add origin`
- [ ] Виконано `git push -u origin main`
- [ ] Активовано GitHub Pages
- [ ] Перевірено, що сайт працює
- [ ] Створено 3 Issues
- [ ] Отримано два посилання для здачі

---

**Успіхів! 🚀**

Якщо виникнуть питання - напишіть мені!

