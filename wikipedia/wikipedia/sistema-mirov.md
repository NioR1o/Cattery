---
icon: globe-pointer
---

# Система миров

Ради наивысшей оптимизации проекта, выживание разделено на два отдельных сервера.

{% hint style="success" %}
Между серверами проходит полная синхронизация игроков:

Здоровье, инвентарь, достижения, атрибуты, сытость.
{% endhint %}

***

### Архитектура проекта:

<table data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td>Сервер: <mark style="background-color:blue;">[Прокси]</mark></td><td>Ядро — Velocity</td><td>Через этот сервер проходят все игроки, он связывает всю сеть проекта</td></tr><tr><td>Сервер: <mark style="background-color:red;">[Построек]</mark></td><td>Ядро — Модифицированный Paper</td><td>Главный сервер для архитектурного творчества игроков</td></tr><tr><td>Сервер: <mark style="background-color:yellow;">[Ферм]</mark></td><td>Ядро — Модифицированный Paper</td><td>Второй сервер, существует для максимально производительных Майнкрафтовских ферм</td></tr><tr><td>Сервер: <mark style="background-color:purple;">[Тестов]</mark></td><td>Ядро — Модифицированный Paper</td><td>Создан для тества плагинов и других механик, перед добавлением на основной сервер. (Курилка админов)</td></tr></tbody></table>

<details>

<summary>Механики Мира: [Построек]</summary>

* Спавн рейт мобов сильно уменьшен
* Фантомы отключены
* У жителей отключен ИИ
* Прорисовка 15 чанков
* Симуляция 5 чанков
* Происходит очистка ентити, расположеных слишком близко

</details>

<details>

<summary>Механики Мира: [Фермы]</summary>

* Спавн рейт мобов увеличен
* Фантомы включены
* Прорисовка 10 чанков
* Симуляция 15 чанков

</details>
