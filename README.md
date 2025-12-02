# 🎮 Kentucky V Launcher

Официальный лаунчер для Kentucky V RAGE MP сервера.

![Kentucky V Launcher](https://img.shields.io/badge/version-1.0.0-orange?style=for-the-badge)
![Electron](https://img.shields.io/badge/Electron-28.0.0-blue?style=for-the-badge&logo=electron)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

## ✨ Особенности

- 🚀 **Быстрый запуск** - Одним кликом подключайтесь к серверу
- 📰 **Новости** - Будьте в курсе последних обновлений
- ⚙️ **Настройки** - Полный контроль над лаунчером
- 📊 **Статистика** - Онлайн игроков и пинг сервера
- 🎨 **Современный дизайн** - Тёмная тема с оранжевыми акцентами
- 🔗 **Быстрые ссылки** - Discord, VK, Форум, Донат

## 📦 Установка

### Предварительные требования

1. Установите [Node.js](https://nodejs.org/) (рекомендуется LTS версия)
2. Установите [Git](https://git-scm.com/)

### Шаги установки

```bash
# 1. Клонируйте репозиторий
git clone https://github.com/20XMAS24/kentucky-launcher.git

# 2. Перейдите в папку проекта
cd kentucky-launcher

# 3. Установите зависимости
npm install

# 4. Запустите лаунчер
npm start
```

## 🛠️ Сборка .exe файла

Для создания готового установщика:

```bash
npm run build
```

Готовый файл будет в папке `dist/`

## ⚙️ Настройка

### Изменение IP сервера

Откройте `index.html` и найдите строку:

```javascript
const SERVER_IP = '185.169.134.78:22005'; // Замените на свой IP
```

### Добавление ресурсов

Создайте папку `assets/` и добавьте:

1. **icon.ico** - Иконка приложения (256x256 px)
2. **background.jpg** - Фоновое изображение GTA 5 (1920x1080 px)

### Изменение ссылок

В `index.html` найдите и измените:

```javascript
openLink('https://discord.gg/kentucky')  // Discord
openLink('https://vk.com/kentuckyv')     // VK
openLink('https://kentuckyv.ru/forum')   // Форум
openLink('https://kentuckyv.ru/donate')  // Донат
```

## 📚 Структура проекта

```
kentucky-launcher/
├── assets/
│   ├── icon.ico           # Иконка приложения
│   └── background.jpg     # Фоновое изображение
├── node_modules/         # Зависимости
├── dist/                 # Готовая сборка
├── .gitignore
├── index.html            # Интерфейс лаунчера
├── main.js               # Основной процесс Electron
├── package.json          # Конфигурация проекта
└── README.md             # Документация
```

## 🎨 Дизайн

Лаунчер выполнен в стиле сайта [kentuckyv.ru](https://kentuckyv.ru):

- **Цветовая схема:**
  - Основной: `#0a0e1a` (тёмно-синий)
  - Акцент: `#ff6b00` (оранжевый)
  - Текст: `#ffffff` (белый)

- **Особенности:**
  - Стеклянные эффекты (glassmorphism)
  - Плавные анимации
  - Адаптивный интерфейс
  - Современные UI-компоненты

## 🔧 Разработка

### Технологии

- **Electron** - Кросс-платформенные десктоп-приложения
- **HTML/CSS/JavaScript** - Интерфейс и логика
- **Electron Builder** - Сборка и дистрибуция

### Команды разработчика

```bash
# Запуск в режиме разработки
npm start

# Сборка приложения
npm run build

# Очистка проекта
rm -rf node_modules dist
```

## ❓ FAQ

### Как изменить цвета?

Откройте `index.html` и измените CSS-переменные:

```css
background: #0a0e1a;              /* Фоновый цвет */
color: #ff6b00;                    /* Акцентный цвет */
border: 1px solid rgba(255, 107, 0, 0.3);  /* Границы */
```

### Почему не запускается игра?

1. Убедитесь, что RAGE MP установлен
2. Проверьте правильность IP-адреса
3. Проверьте статус сервера

### Как добавить автообновление?

Используйте [electron-updater](https://www.electron.build/auto-update) для реализации автоматических обновлений.

## 👥 Контакты

- **Сайт:** [kentuckyv.ru](https://kentuckyv.ru)
- **Discord:** [discord.gg/kentucky](https://discord.gg/kentucky)
- **VK:** [vk.com/kentuckyv](https://vk.com/kentuckyv)
- **GitHub:** [github.com/20XMAS24/kentucky-launcher](https://github.com/20XMAS24/kentucky-launcher)

## 📜 Лицензия

MIT License

## 🎉 Благодарности

- **Electron** - За отличный фреймворк
- **RAGE MP** - За платформу мультиплеера
- **Kentucky V Team** - За удивительный сервер

---

<div align="center">
  <b>Сделано с ❤️ для Kentucky V RolePlay</b>
</div>