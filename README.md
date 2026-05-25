```markdown
# ⚡ WAS v3 — Windows Activation Script

[![GitHub stars](https://img.shields.io/github/stars/windusik/was-v3?style=for-the-badge&color=blue)](https://github.com/windusik/was-v3/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/windusik/was-v3?style=for-the-badge&color=green)](https://github.com/windusik/was-v3/network)
[![GitHub license](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](https://github.com/windusik/was-v3/blob/main/LICENSE)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011%20%7C%20Server-blue?style=for-the-badge&logo=windows)](https://github.com/windusik/was-v3)

> **Легкий, мощный и безопасный инструмент для активации Windows и Office**

---

## 📌 О проекте

**WAS v3** — это универсальный скрипт для активации продуктов Microsoft.  
Он объединяет все современные методы активации в одном простом меню.

### ✨ Особенности

| Метод | Поддержка | Описание |
|-------|-----------|----------|
| **HWID** | Windows 10/11 | Цифровая лицензия (навсегда) |
| **Ohook** | Office | Постоянная активация Office |
| **TSforge** | Windows / Office / ESU | Универсальный метод для любых версий |
| **Online KMS** | Windows / Office | Классическая KMS-активация |

### 🚀 Преимущества

- ✅ **100% безопасность** — скрипт не содержит вредоносного кода
- ✅ **Работает без интернета** — некоторые методы не требуют сети
- ✅ **Поддержка всех версий** — от Windows 7 до Windows 11 и Server 2025
- ✅ **Автообновление** — всегда актуальная версия
- ✅ **Плановое задание** — автоматическое продление активации (для KMS)

---

## 📥 Установка и запуск

### Способ 1 — GitHub (рекомендуемый)

```powershell
# Откройте PowerShell от имени администратора и выполните:
irm https://github.com/windusik/was-v3/raw/main/MAS_AIO.cmd | iex
```

### Способ 2 — Скачать вручную

1. Перейдите в [релизы](https://github.com/windusik/was-v3/releases)
2. Скачайте `WAS_v3_AIO.cmd`
3. Запустите **от имени администратора**

### Способ 3 — Клонировать репозиторий

```bash
git clone https://github.com/windusik/was-v3.git
cd was-v3
# Запустите MAS_AIO.cmd от имени администратора
```

---

## 🎮 Использование

### Интерактивный режим

Просто запустите скрипт и выберите нужный пункт меню:

```
=============================================================
    [1] HWID                - Windows
    [2] Ohook               - Office  
    [3] TSforge             - Windows / Office / ESU
    [4] Online KMS          - Windows / Office
    [5] Check Activation Status
    [6] Change Windows Edition
    [7] Change Office Edition
    [0] Exit
=============================================================
```

### Автоматический режим (параметры командной строки)

```cmd
# Активация через HWID
MAS_AIO.cmd /HWID

# Активация Office через Ohook
MAS_AIO.cmd /Ohook

# Активация через TSforge
MAS_AIO.cmd /Z-Windows

# KMS-активация всего
MAS_AIO.cmd /K-WindowsOffice

# Удалить KMS-активацию
MAS_AIO.cmd /K-Uninstall

# Создать $OEM$ папку для автоматической активации при установке
MAS_AIO.cmd /HWID /Ohook
```

### Параметры TSforge

| Параметр | Описание |
|----------|----------|
| `/Z-Windows` | Активация Windows |
| `/Z-ESU` | Активация ESU-обновлений |
| `/Z-Office` | Активация Office |
| `/Z-Reset` | Сброс счетчиков активации |
| `/Z-SCID` | StaticCID метод (требует интернет) |
| `/Z-ZCID` | ZeroCID метод |
| `/Z-KMS4k` | KMS4k метод (активация на 4000+ лет) |

---

## 🛠️ Требования

| Компонент | Минимальная версия |
|-----------|-------------------|
| Windows | Vista SP2 и выше |
| PowerShell | 2.0 и выше |
| .NET Framework | 3.5 и выше |
| Права | Администратор |

---

## 📂 Структура репозитория

```
was-v3/
├── MAS_AIO.cmd          # Основной скрипт
├── LICENSE              # Лицензия MIT
├── README.md            # Этот файл
└── BIN/                 # (опционально) Пользовательские DLL
    ├── sppc32.dll
    └── sppc64.dll
```

---

## ❓ Частые вопросы

### ❔ Безопасно ли это?

**Да.** Код скрипта полностью открыт. Вы можете сами убедиться, что в нем нет вредоносного кода.  
Единственное, что делает скрипт — активирует Windows/Office через штатные механизмы Microsoft.

### ❔ Почему антивирус ругается?

Некоторые антивирусы могут ложно срабатывать на скрипты активации.  
Добавьте папку со скриптом в исключения или временно отключите защиту.

### ❔ Нужно ли переустанавливать систему при смене редакции?

Нет. Скрипт меняет редакцию Windows на лету.

### ❔ Как удалить KMS-активацию?

Запустите скрипт → выберите `Online KMS` → пункт `Uninstall Online KMS`

---

## 🤝 Как помочь проекту

⭐ **Поставьте звезду на GitHub** — это мотивирует развивать проект дальше!

Также вы можете:
- Сообщать об ошибках в [Issues](https://github.com/windusik/was-v3/issues)
- Предлагать новые функции
- Делиться проектом с друзьями

---

## 📜 Лицензия

Проект распространяется под лицензией **MIT**.  
Вы можете свободно использовать, модифицировать и распространять скрипт.

---

## 🔗 Ссылки

- 🌐 [Репозиторий на GitHub](https://github.com/windusik/was-v3)
- ⭐ [Поставить звезду](https://github.com/windusik/was-v3/stargazers)

---

<p align="center">
  <b>Made with ❤️ for the community</b><br>
  <sub>© 2026 WAS v3 — Free and Open Source Software</sub>
</p>
```
