# Создание проекта Django
> Основные задачи:
> - Создать проект Django
> - Добавить в него 3 статические странички
> - На одной из страниц контент повторяется 2 раза без изменения content (два раза прописано {{ flatpage.content }})
> - Одна из страниц на сайте доступна только админу (только вошедшему пользователю)
> - На одной из страниц изменены шрифты и размеры текста
> - Сайт представляет собой оформленный Bootstrap-шаблон со встроенными пользовательскими данными
> - Статические файлы Bootstrap загружаются через теги {% load static %} и {% static %}

Реализация и пояснения по кроекту:
1. Шаблон contact_page.html изменен умышленно (с тегом extends и блоками content), чтобы шапочка была 💂‍♂
2. Cозданы три страницы (product, service, special) и они выведены в шапочку, чтобы можно было тыкать 🐁:
  - Страница product пустая, но с шапкой. И поскольку на ней условная запрещёнка — страница доступна только зарегистрированным пользователям 🔞
  - Страница service не только с шапкой, но и блоками content. Сам контент цветаст, привлекателен и содержателен 🍓
  - Страница special без шапки. Зато на ней всё по два, ибо акционная 🌭 🌭
3. Из папки static удалено всё, кроме папки css с соответствующим файлом styles 🎩
