# Yandex Music Playlist Exporter — Instruction 

The entire script was created using AI.
---

## Как воспользоваться скриптом (на русском)

**Кратко:**  
Этот скрипт выгружает твой плейлист Яндекс Музыки в TXT/CSV, даже с локальными и битым треками.  
Просто замени файл artist.py в папке site-packages, запусти скрипт с токеном — получи полный список и таблицу!

### 1. Установи Python  
Скачай с [python.org](https://www.python.org/downloads/), установи, добавь в PATH.

### 2. Поставь yandex-music  
pip install yandex-music

text

### 3. Замени artist.py  
- Найди:
C:\Users<ТВОЁ_ИМЯ>\AppData\Local\Programs\Python\Python3X\Lib\site-packages\yandex_music\artist\

text
- Копируй новый artist.py, согласись на замену.

### 4. Получи токен  
Инструкция:  
[https://github.com/MarshalX/yandex-music-api/discussions/513](https://github.com/MarshalX/yandex-music-api/discussions/513)

### 5. Запускай скрипт!
python yandex_exporter.py --token ТВОЙ_ТОКЕН --url "ССЫЛКА_НА_ПЛЕЙЛИСТ" --out список.txt --csv таблица.csv

text
- `--limit 100` — ограничить выгрузку
- `--filter "Artist"` — только треки по слову
- `--dedup` — убрать дубли

### 6. Получи TXT и таблицу CSV (Excel/Sheets)!

**Если что-то не работает:**  
Проверь замену, путь, токен, ссылку.  
Вопросы — можешь писать!

---

## English quick guide

**How to use:**
- This script exports any Yandex Music playlist (even broken or local tracks) to TXT/CSV.
- Replace `artist.py` in your Python `site-packages`.
- Install yandex-music:  
pip install yandex-music

text
- Get your Yandex Music API token (see: [https://github.com/MarshalX/yandex-music-api/discussions/513](https://github.com/MarshalX/yandex-music-api/discussions/513)).
- Run:
python yandex_exporter.py --token YOUR_TOKEN --url "YOUR_PLAYLIST_URL" --out list.txt --csv table.csv

text
- Options:  
`--limit`, `--filter "word"`, `--dedup`
- Result: TXT (for reading), CSV (Excel, Google Sheets, supports Unicode).

**Troubles?**  
- Make sure you replaced artist.py correctly.
- Double-check paths, token, and playlist link.

---
