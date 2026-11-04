<div align="center">

# Crystal Messenger

**A simple messenger for web, Android and Windows.**
**Простой мессенджер для браузера, Android и Windows.**

[English](#english) · [Русский](#русский)

</div>

---

## English

Crystal is a small messenger I build for everyone who wants a calm place to talk: no ads, no feed, no algorithm. It is in **closed beta**.

### Download

Get the latest build from the [Releases](https://github.com/Pashamin/Crystal/releases/latest) page:

| Platform | File |
|---|---|
| Android | `Crystal-<version>.apk` |
| Windows | `Crystal-<version>-setup.exe` |
| Browser | <https://crystalmessenger-beta.web.app> |

The builds are **not signed yet**, so the system will warn you. That is expected for a beta:

- **Windows:** in the SmartScreen window press **More info**, then **Run anyway**.
- **Android:** allow installing from this source. If Play Protect complains, choose **Install anyway**.

### Access

While the beta is small (up to about 100 people), signing in requires an invitation key. You can request one inside the app after you create an account. Keys are one-time and checked on the server side.

### Features

- Direct chats, groups with descriptions, a shared channel, news and private notes
- Voice messages, several attachments per message, an audio player
- Replies with a jump to the original, forwarding, editing, reactions, pinned messages
- Message search and per-chat drafts
- Three interface styles, OLED / graphite / light surfaces, accent colors, avatar shapes and corner radius
- PIN lock; new-device sign-in alerts with a one-tap "not me" that signs out every device
- Push notifications on Android, native notifications on Windows, one-tap in-app updates
- Russian and English sign-in screens (the rest of the interface is being translated)

### Built with

React 19, Vite, Tailwind CSS 4, Firebase (Auth, Firestore, App Check, Hosting), Capacitor 8 (Android), Tauri 2 and Rust (Windows). There is no custom backend server: data lives in Firebase, and push notifications are sent by a small Node.js worker running in Docker on a home server.

### Good to know

- **No end-to-end encryption.** Messages are protected in transit and by database rules, but the person who runs the database can technically read them. Do not use Crystal for anything that must stay secret.
- This is a beta: things will break and change. Found a bug or have an idea? There is a feedback form in the app settings.
- **Source code** is not published yet. This repository currently hosts releases. The code will be opened later.

---

## Русский

Crystal — небольшой мессенджер, который я делаю для всех, кому нужно спокойное место для общения: без рекламы, ленты и алгоритмов. Сейчас идёт **закрытая бета**.

### Скачать

Свежая версия лежит на странице [Releases](https://github.com/Pashamin/Crystal/releases/latest):

| Платформа | Файл |
|---|---|
| Android | `Crystal-<версия>.apk` |
| Windows | `Crystal-<версия>-setup.exe` |
| Браузер | <https://crystalmessenger-beta.web.app> |

Сборки **пока без подписи**, поэтому система предупредит. Для беты это нормально:

- **Windows:** в окне SmartScreen нажмите **Подробнее**, затем **Выполнить в любом случае**.
- **Android:** разрешите установку из этого источника. Если Play Protect ругается, выберите **Всё равно установить**.

### Доступ

Пока бета небольшая (до 100 человек), для входа нужен ключ-приглашение. Запросить его можно прямо в приложении после регистрации. Ключи одноразовые и проверяются на стороне сервера.

### Возможности

- Личные чаты, группы с описанием, общий канал, новости и личные заметки
- Голосовые сообщения, несколько вложений в одном сообщении, плеер аудио
- Ответы с переходом к оригиналу, пересылка, правка, реакции, закреп
- Поиск по сообщениям и черновики для каждого чата
- Три стиля интерфейса, чёрная, графитовая и светлая поверхность, акценты, форма аватарок и скругление
- ПИН-блокировка; уведомления о входе с нового устройства и кнопка «не я», которая выходит со всех устройств
- Push на Android, уведомления на Windows, обновление в одно нажатие
- Экраны входа на русском и английском (остальной интерфейс переводится)

### Из чего сделано

React 19, Vite, Tailwind CSS 4, Firebase (вход, Firestore, App Check, хостинг), Capacitor 8 (Android), Tauri 2 и Rust (Windows). Своего сервера нет: данные в Firebase, а push рассылает небольшой воркер на Node.js в Docker на домашнем сервере.

### Что важно знать

- **Нет сквозного шифрования.** Сообщения защищены при передаче и правилами базы, но тот, кто управляет базой, технически может их прочитать. Не используйте Crystal для того, что должно остаться секретом.
- Это бета: что-то будет ломаться и меняться. Нашли баг или есть идея? В настройках приложения есть форма обратной связи.
- **Исходный код** пока не опубликован. Сейчас в этом репозитории лежат релизы, а код будет открыт позже.
