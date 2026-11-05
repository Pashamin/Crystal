<div align="center">

# Crystal Messenger

**A simple messenger for web, Android and Windows.**
**Простой мессенджер для браузера, Android и Windows.**

[English](#english) · [Русский](#русский)

🌐 **Website / Сайт:** <https://crystal-site.web.app>

</div>

---

## English

Crystal is a simple messenger for everyone who wants a calm place to talk: no ads, no feed, no algorithm. It is in **closed beta**. More about it on the [website](https://crystal-site.web.app).

### Download

Get the latest build from the [Releases](https://github.com/Pashamin/Crystal/releases/latest) page:

| Platform | File |
|---|---|
| Android | `Crystal-<version>.apk` |
| Windows | `Crystal-<version>-setup.exe` |
| Browser | <https://crystalmessenger-beta.web.app> |
| Website | <https://crystal-site.web.app> (features, version history, downloads) |

The builds are **not signed yet**, so the system will warn you. That is expected for a beta:

- **Windows:** in the SmartScreen window press **More info**, then **Run anyway**.
- **Android:** allow installing from this source. If Play Protect complains, choose **Install anyway**.

### Access

While the beta is small (up to about 100 people), signing in requires an invitation key. Open the app, create an account, and it will offer to request a key. Keys are one-time and checked on the server side.

### Features

- Direct chats, groups you can rename and describe, a shared channel with an unread counter, news and private notes
- Voice messages, several attachments per message, an audio player
- Replies with a jump to the original, forwarding, editing, reactions, pinned messages
- Message search; drafts for every chat, shown in the chat list
- Three interface styles, OLED / graphite / light surfaces, accent colors, avatar shapes and corner radius
- PIN lock; new-device sign-in alerts with a one-tap "not me" that signs out every device
- Push notifications on Android: unread messages are combined into one notification with pictures; `@mentions` in the shared chat; native notifications on Windows; one-tap in-app updates
- Mute notifications everywhere or per chat: for an hour, a day, a week or until you turn them back on (synced across your devices)
- A compact chat menu on phones
- The interface is in Russian

### Built with

React 19, Vite, Tailwind CSS 4, Firebase (Auth, Firestore, App Check, Hosting), Capacitor 8 (Android), Tauri 2 and Rust (Windows). There is no custom backend server: data lives in Firebase, and push notifications are sent by a small Node.js worker running in Docker on our own server.

### Good to know

- **No end-to-end encryption.** Messages are protected in transit and by database rules, but the person who runs the database can technically read them. Do not use Crystal for anything that must stay secret.
- This is a beta: things will break and change. Found a bug or have an idea? There is a feedback form in the app settings.
- **Source code** is not published yet. This repository currently hosts releases. The code will be opened later.

---

## Русский

Crystal — простой мессенджер для всех, кому нужно спокойное место для общения: без рекламы, ленты и алгоритмов. Сейчас идёт **закрытая бета**. Подробнее на [сайте](https://crystal-site.web.app).

### Скачать

Свежая версия лежит на странице [Releases](https://github.com/Pashamin/Crystal/releases/latest):

| Платформа | Файл |
|---|---|
| Android | `Crystal-<версия>.apk` |
| Windows | `Crystal-<версия>-setup.exe` |
| Браузер | <https://crystalmessenger-beta.web.app> |
| Сайт проекта | <https://crystal-site.web.app> (возможности, история версий, скачивание) |

Сборки **пока без подписи**, поэтому система предупредит. Для беты это нормально:

- **Windows:** в окне SmartScreen нажмите **Подробнее**, затем **Выполнить в любом случае**.
- **Android:** разрешите установку из этого источника. Если Play Protect ругается, выберите **Всё равно установить**.

### Доступ

Пока бета небольшая (до 100 человек), для входа нужен ключ-приглашение. Откройте приложение, создайте аккаунт, и оно предложит запросить ключ. Ключи одноразовые и проверяются на стороне сервера.

### Возможности

- Личные чаты, группы с названием и описанием (их можно менять), общий канал со счётчиком новых сообщений, новости и личные заметки
- Голосовые сообщения, несколько вложений в одном сообщении, плеер аудио
- Ответы с переходом к оригиналу, пересылка, правка, реакции, закреп
- Поиск по сообщениям; черновики для каждого чата, видны в списке чатов
- Три стиля интерфейса, чёрная, графитовая и светлая поверхность, акценты, форма аватарок и скругление
- ПИН-блокировка; уведомления о входе с нового устройства и кнопка «не я», которая выходит со всех устройств
- Push на Android: непрочитанные сообщения собраны в одно уведомление, картинки видны; упоминания `@ник` в общем чате; уведомления на Windows; обновление в одно нажатие
- Отключение уведомлений везде или в одном чате: на час, день, неделю или до включения (синхронизируется между вашими устройствами)
- Компактное меню чата на телефоне
- Интерфейс на русском

### Из чего сделано

React 19, Vite, Tailwind CSS 4, Firebase (вход, Firestore, App Check, хостинг), Capacitor 8 (Android), Tauri 2 и Rust (Windows). Своего сервера нет: данные в Firebase, а push рассылает небольшой воркер на Node.js в Docker на собственном сервере.

### Что важно знать

- **Нет сквозного шифрования.** Сообщения защищены при передаче и правилами базы, но тот, кто управляет базой, технически может их прочитать. Не используйте Crystal для того, что должно остаться секретом.
- Это бета: что-то будет ломаться и меняться. Нашли баг или есть идея? В настройках приложения есть форма обратной связи.
- **Исходный код** пока не опубликован. Сейчас в этом репозитории лежат релизы, а код будет открыт позже.
