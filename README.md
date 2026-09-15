<div align="center">

  <h1>He_Trogati_Mne</h1>
  <p><b>«digital footprint // leave no trace» // nothing else matters</b></p>

  <p>
    <a href="https://twitter.com/He_Trogati_Mne"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
    <a href="https://instagram.com/He_Trogati_Mne"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" /></a>
    <a href="https://tiktok.com/@he_trogati_mne"><img src="https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white" alt="TikTok" /></a>
    <a href="https://youtube.com/@he_trogati_mne"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube" /></a>
    <a href="https://twitch.tv/He_Trogati_Mne"><img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" alt="Twitch" /></a>
    <a href="https://open.spotify.com/user/31b6kcuj5au3c3qdehos2tprxtxu"><img src="https://img.shields.io/badge/Spotify-1ED760?style=for-the-badge&logo=spotify&logoColor=white" alt="Spotify" /></a>
    <a href="https://soundcloud.com/He_Trogati_Mne"><img src="https://img.shields.io/badge/SoundCloud-FF5500?style=for-the-badge&logo=soundcloud&logoColor=white" alt="SoundCloud" /></a>
    <a href="https://discord.gg/DQHpbet36W"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
    <a href="https://github.com/He-Trogati-Mne"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
    <a href="https://reddit.com/user/He_Trogati_Mne/"><img src="https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white" alt="Reddit" /></a>
  </p>

</div>

---

## Про проєкт

**MOON** — персональна стартова сторінка браузера (Bio Link / Linktree Alternative), виконана в темному мінімалістичному стилі з елементами термінального інтерфейсу, ASCII-графіки та glassmorphism.

Сторінка об'єднує всі медіа-ресурси, соціальні мережі та вбудований аудіоплеєр в одному вікні — як домашня сторінка замість стандартного new tab.

---

## Можливості

### Основне
- **Кастомізований ASCII-об'єкт** у шапці — Місяць / Сатурн / Земля з обертанням у реальному часі
- **Живий годинник + погода** для будь-якого міста світу (віджет у шапці)
- **Пошукова строка** з підтримкою Google / Bing / DuckDuckGo / Yahoo / Ecosia
- **Голосовий пошук** (Web Speech API)
- **Пошук за зображенням** (Google Lens)
- **Закладки (shortcuts)** з drag & drop, підтримкою favicon та контекстним меню
- **Музичний плеєр** з підтримкою SoundCloud, Spotify, YouTube, YouTube Music

---

### Фон та візуальні ефекти
- Відеофон / картинка / iframe (YouTube, TikTok, Vimeo, будь-який сайт)
- Drag & drop файлів прямо у вікно
- Налаштування розмиття, затемнення, віньєтування, кольору фону
- **20+ ефектів заголовка**: градієнт, неон, вогонь, лід, веселка, голографія, глітч, ретро, тиснення, гравіювання, пульсація, мерехтіння тощо

### Кастомізація
- Вибір шрифту з **28 шрифтів Google Fonts**
- Налаштування розмірів, відступів, радіусів, прозорості та розмиття блоків
- Зміна розташування плеєра (inline або фіксоване у 9 позиціях + власна)
- **Режим перетягування блоків** — зміна порядку елементів мишкою
- Збереження всіх налаштувань у `localStorage`

### Інше
- Локалізація: **українська / англійська**
- **Панель Google-додатків** (9 точок) — швидкий доступ до Gmail, Карт, Диску, Календаря, YouTube тощо
- Адаптивна верстка під мобільні пристрої
- Кастомний SVG-фавікон

---

## Технології

- **HTML5 / CSS3** — без фреймворків
- **Vanilla JavaScript** — без бібліотек
- **ASCII Raycaster** — власна реалізація 3D-рендерингу планет на `<pre>`
- **SoundCloud Widget API** — для повного контролю над плеєром
- **Spotify IFrame API** + fallback на embed
- **YouTube IFrame API** + fallback на embed
- **Open-Meteo API** — погода без ключів
- **Google Fonts** — 28 шрифтів
- **Google Apps CDN** — іконки сервісів

---

## Швидкий старт

### Варіант 1 — GitHub Pages (рекомендовано)

1. Форкніть або клонуйте репозиторій
2. Завантажте файли в репозиторій
3. **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save**
4. Через 1–2 хвилини сайт буде доступний за адресою:
https://ваш-нік.github.io/назва-репозиторію/

**Важливо:** саме HTTPS з GitHub Pages потрібен для коректної роботи Spotify / YouTube IFrame API та Web Speech API (мікрофон).

### Варіант 2 — локально

Через `file://` працюють не всі функції (Spotify / YouTube API, мікрофон). Рекомендується локальний сервер:

```bash
python -m http.server 8000
Або Live Server у VS Code, але обов'язково з хостом localhost:
http://localhost:8000/index.html
⚠️ 127.0.0.1 не працює зі Spotify IFrame API — використовуйте саме localhost.
```

---

## Часть 7 — Структура проекта

```markdown
## Структура проєкту
.
├── index.html # Головна сторінка з усім функціоналом
├── biolink.html # Альтернативна сторінка з посиланнями (bio link)
└── README.md # Цей файл
```

---

## Соціальні мережі

| Платформа | Посилання |
| :--- | :--- |
| **X / Twitter** | [twitter.com/He_Trogati_Mne](https://twitter.com/He_Trogati_Mne) |
| **Instagram** | [instagram.com/He_Trogati_Mne](https://instagram.com/He_Trogati_Mne) |
| **TikTok** | [tiktok.com/@he_trogati_mne](https://tiktok.com/@he_trogati_mne) |
| **YouTube** | [youtube.com/@he_trogati_mne](https://youtube.com/@he_trogati_mne) |
| **Twitch** | [twitch.tv/He_Trogati_Mne](https://twitch.tv/He_Trogati_Mne) |
| **Spotify** | [open.spotify.com/user/31b6kcuj5au3c3qdehos2tprxtxu](https://open.spotify.com/user/31b6kcuj5au3c3qdehos2tprxtxu) |
| **SoundCloud** | [soundcloud.com/He_Trogati_Mne](https://soundcloud.com/He_Trogati_Mne) |
| **GitHub** | [github.com/He-Trogati-Mne](https://github.com/He-Trogati-Mne) |
| **Reddit** | [reddit.com/user/He_Trogati_Mne](https://reddit.com/user/He_Trogati_Mne/) |

---

## Ліцензія

Особистий проєкт. Використовуйте як захочете — форкніть, змініть під себе, розгорніть у себе. Але не забувайте про `// leave no trace`.

---

<div align="center">

**MOON** · _nothing else matters_

</div>
