---
description: Информация по командам и список команд
cover: ../../../.gitbook/assets/bg for document.png
coverY: -30
layout:
  width: default
  cover:
    visible: true
    size: hero
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
  metadata:
    visible: true
---

# Команды

## Важные моменты

### 1. Права использования команд

Не используйте команды не по назначению, для собственного развлечения без разрешения руководства и не тестируйте их на общедоступных серверах.

{% hint style="info" %}
Для тестирования команд есть сервер [**AdminOnly**](#user-content-fn-1)[^1]
{% endhint %}

### 2. Аргументы команд

Некоторые команды требуют обязательное указание аргументов или могут использовать дополнительные аргументы.

<kbd>( )</kbd> - обязательный аргумент

<kbd>< ></kbd> - необязательный аргумент

{% hint style="info" %}
**Пример**

Аргументы команды `ban` выглядят так `(UserId/PlayerId/IpAddress) (время) (причина)`

Значит для команды обязательно нужно **3** аргумента.

Примерный ввод команды `ban` должен выглядеть так `ban 3 50y Читы`
{% endhint %}

### 3. Идентификаторы

Для обращения к конкретным игрокам через команды используются особые идентификаторы.

* **UserId**\
  Id пользователя в одной из 3-х систем (Steam, Discord и Northwood).\
  Состоит из префикса (число или символы) и постфикса (@steam, @discord и @northwood).\
  **Пример:** 76561199500773801@steam
* **PlayerId**\
  Id игрока на сервере или просто игровой Id. Состоит только из числа.\
  **Пример:** 5
* **Ip-Address**
* **Nickname**

### **4. Алиасы**

У некоторых команд имеются алиасы[^2], что позволяет быстрее вводить такие команды.

## Список команд

<table data-view="cards" data-full-width="false"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td><a data-mention href="osnovnye-komandy.md">osnovnye-komandy.md</a></td><td><a href="osnovnye-komandy.md">osnovnye-komandy.md</a></td><td><a href="../../../.gitbook/assets/bob_thinking.png">bob_thinking.png</a></td></tr><tr><td><a data-mention href="funtoolbox.md">funtoolbox.md</a></td><td></td><td><a href="../../../.gitbook/assets/bob_smiles.png">bob_smiles.png</a></td></tr></tbody></table>

[^1]: Приватный сервер для сотрудников проекта, на который можно подключиться только напрямую через Ip-Адрес

[^2]: Альтернативные названия команды
