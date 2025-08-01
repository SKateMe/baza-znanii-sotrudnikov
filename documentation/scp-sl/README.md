---
description: Документации для SCP:SL
icon: box
coverY: 0
layout:
  width: default
  cover:
    visible: false
    size: full
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# SCP:SL

## 1. Основная информация&#x20;

**Администраторам строго запрещается использовать любые из нижеперечисленных команд для собственного развлечения и тестирования их функций. Информация ниже предоставлена в ознакомительных целях.**

Админ. панель (RA) предоставляет пользователю множество функций, которых должно быть достаточно для большинства нужд администрации. Перед тем, как заняться непосредственно описанием этих функций, стоит упомянуть несколько вещей, которые не нашли места для описания ниже:

{% hint style="success" %}
* Открыть админ табличку вы можете нажав на латинскую \[M]
* Вы можете выбрать несколько игроков, нажимая на них с зажатой клавишей \[Ctrl]
* Всегда проверяйте, где находится выделение, так как после закрытия таблички его положение может не сбрасываться до конца раунда
* Для доступа в REMOTE ADMIN консоль нужно мышкой нажать на пункт \[Open text-based remote admin version], при нажатии на \[\~] у вас открывается не RA, а обычная консоль пользователя
* Чтобы выбрать всех игроков, нужно выбрать одного игрока и нажать одновременно \[CTRL] + \[A]
* Чтобы активировать префикс на сервере, нужно прописать команду tag в консоли на \[ \~ ], чтобы убрать префикс, пропишите команду higetag в консоли на \[ \~ ]
{% endhint %}

{% hint style="warning" %}
**Примечания:**&#x20;

* PlayerId / ID Игрока - это внутриигровой id на сервере (не путать со SteamID и DiscordID)
* ( )/<> - это обязательный/необязательный аргумент для команды, который необходимо указывать без скобок (пример: log разборки)
* Проверить команды и их работоспособность вы можете на сервере admin-only, на который можно зайти только через IP сервера
{% endhint %}

## Команды RA

### hidetag/showtag

Скрывает ваш префикс от игроков. Администрация по прежнему видит ваш префикс. / Возвращает ваш скрытый префикс.

### punishments

Выводит список наказаний у игрока с указанными параметрами.&#x20;

Работает по шаблону `punishments (PlayerId или UserID) <Ban.ForceWarn.Warn> <Порты серверов> <Максимум вхождений> <Номер страницы>`

### warns

Выводит список предупреждений у игрока с указанными параметрами.

Работает по шаблону `warns (PlayerId или UserID) <Порты серверов> <Максимум вхождений> <Номер страницы>`

### warn&#x20;

Выдаёт предупреждению игроку. Предупреждение отображается у игрока в игровой консоли на ''\~''

Работает по шаблону `warn (PlayerId) (причина)`

### delwarn&#x20;

Удаляет предупреждение из списка наказаний игрока&#x20;

Работает по шаблону `delwarn (ID наказания) (причина)`

### bans

Выводит список банов у игрока с указанными параметрами.

Работает по шаблону `bans (PlayerId или UserID) <Порты серверов> <Максимум вхождений> <Номер страницы>`

### ban&#x20;

Блокирует игроку доступ к серверу, на котором было выдано наказание.

Работает по шаблону `ban (PlayerId / UserId / Ip-адрес) (время) (причина)`

{% hint style="info" %}
**Индексы времени:**

* m - минута
* h - час
* d - день
* M - месяц
* y - год&#x20;
{% endhint %}

### unban&#x20;

Снимает у игрока блокировку по указанному steamid64 или IP адресу.

Работает по шаблону `unban (id/ip) (SteamId64 / IP-адрес)`

### forcewarnings

Выводит список переводов игрока в наблюдатели за определённое кол-во дней. Изначально за 3 дня.

Работает по шаблону `forcewarnings (PlayerId или UserID) <Порты серверов> <Максимум вхождений> <Номер страницы>`&#x20;

### forcewarn

Выдает игроку предупреждение, после чего переводит его в наблюдатели.

Работает по шаблону `forcewarn (PlayerId) (причина)`

### nicknamesblacklist

Выводит в RA консоли информацию о заблокированных никнеймах.

### addblacklistword&#x20;

Вносит элемент в список заблокированных никнеймов.

Работает по шаблону `addblacklistword (элемент)`

### removeblacklistword

Удаляет элемент из списка заблокированных никнеймов.

Работает по шаблону `removeblacklistword (элемент)`
