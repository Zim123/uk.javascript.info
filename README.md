# Сучасний посібник по JavaScript українською мовою

В цьому репозиторію зберігається переклад <https://javascript.info> на українську мову.

**Ось як ви можете допомогти:**

- Перегляньте першу issue: [Ukrainian Translate Progress](https://github.com/javascript-tutorial/uk.javascript.info/issues/1).
- Виберіть розділ, який ви хочете перекласти. Вибирайте з тих розділів, які ще не відмічені і не перекладаються.
- Додайте коментар до issue, щоб проінформувати інших, що ви перекладаєте цей розділ.
- Створіть форк репозиторію, перекладіть один розділ і коли завершите, надішліть запит на злиття (PR).

За бажанням можете [створити issue](https://github.com/javascript-tutorial/uk.javascript.info/issues/new) із назвою перекладу, наприклад: "Translation: Code quality > Debugging in Chrome".

**Дайте іншим зрозуміти, що ви перекладаєте. Найкращим способом буде написання коментаря до [цього issue](https://github.com/javascript-tutorial/uk.javascript.info/issues/1).**

🎉 Дякуємо!

Ваше ім'я та ваш вклад в переклад з'являться на сторінці "Про проект", коли переклад буде опубліковано.

Якщо ви хочете стати супроводжуючим (maintainer), мати повний доступ до репозиторію і переглядати переклади інших, [створіть нову issue](https://github.com/javascript-tutorial/translate/issues/new) в головному репозиторію, із заголовком "Become maintainer (Ukrainian)".

P.S. Весь перелік мов можна знайти на сторінці <https://javascript.info/translate>.

## Внески

Ми також хочемо, щоб інші люди робили свій вклад в цей посібник.

Якщо ви замітили неточності в перекладі, або ви знаєте нову інформацію, тоді, будь ласка, поділіться цим з іншими людьми (у вигляді запиту на злиття - PR) 👏

**Ви можете редагувати текст в будь-якому редакторі.** Цей посібник використовує формат "markdown", який легко зрозуміти. Якщо ви хочете переглянути, як переклад буде виглядати на сайті, для цього є веб-сервер, який ви можете запустити локально: <https://github.com/javascript-tutorial/server>.

Ось тут перелік людей, які вклали свій час у розвиток цього посібника: <https://javascript.info/about#contributors>.

## Структура

Кожен розділ, стаття або завдання знаходяться у власних папках.

Папка називається в форматі `N-code-editors`, де `N` – це номер для сортування (статті впорядковані), і `code-editors` це частина URL на сайті.

Перегляньте <https://javascript.info/translate> для подробиць.

Папка має один з цих файлів:

- `index.md` якщо це розділ,
- `article.md` якщо стаття,
- `task.md` для формулювання завдання (+`solution.md` з текстом вирішення завдання).

Файл починається із `# Заголовка`; потім йде текст в форматі Markdown, який легко редагується в звичайному текстовому редакторі.

Додаткові ресурси та приклади до статтей або завдань також розміщуються в одній папці.

## Підказки щодо перекладу

- Переклад не обов'яково повинен бути дослівним. Він повинен бути технічно корректним і повинен бути добре зрозумілим.
- Якщо ви бачите, що англійську версію можна вдосконалити - чудово, будь ласка, надішліть PR із правками.

**Будь ласка, зберігайте перенесення рядків і абзаци "як є": не додавайте нові рядки і не видаляйте існуючі.** Це полегшує об'єднання майбутніх змін в англійській версії з цим перекладом.

### Глосарій (словник)

Є деякі слова, які викликають сумніви щодо перекладу. Наприклад, слово "application" - це "програма", "додаток" чи "застосунок"?

Щоб зберегти цілісніть перекладу поміж усіма статтями необхідно вживати однаковий переклад таких слів.

Тому перед перекладом слід ознайомитися із [глосарієм](https://github.com/javascript-tutorial/uk.javascript.info/issues/8).
В процесі перекладу вам можуть зустрітися й інші такі слова. У випадку сумнівів щодо перекладу таких слів – сміливо додавайте їх в глосарій.

### Текст в блоках коду

- Перекладайте коментарі до коду.
- Перекладайте повідомлення користувачів і тестові рядки.
- Не перекладайте змінні, класи, ідентифікатори.
- Переконайтеся, що код працює після перекладу :)

Наприклад:

```js
// Example
const text = "Hello, world";
document.querySelector('.hello').innerHTML = text;
```

✅ Перекладіть коментар і рядок:

```js
// Приклад
const text = 'Привіт, світ';
document.querySelector('.hello').innerHTML = text;
```

❌ Не перекладайте назву класу:

```js
// Приклад
const text = 'Привіт, світ';
// ".hello" це клас
// НЕ ПЕРЕКЛАДАЙТЕ ТАК
document.querySelector('.привіт').innerHTML = text;
```

### Зовнішні посилання

Якщо зовнішнє посилання на Вікіпедію має відповідну українську версію, і ця версія містить досить повну інформацію, в такому випадку варто вказати посилання на українську версію.

Наприклад:

```md
[JavaScript](https://en.wikipedia.org/wiki/JavaScript) is a programming language.
```

✅ Можна замінити на (en -> uk):

```md
[JavaScript](https://uk.wikipedia.org/wiki/JavaScript) це прототипна мова програмування.
```

Якщо посилання на українську версію містить кодовані букви (`https://uk.wikipedia.org/wiki/V8_(%D1%80%D1%83%D1%88%D1%96%D0%B9_JavaScript`), їх слід замінити на українські букви (`https://uk.wikipedia.org/wiki/V8_(рушій_JavaScript)`).

Для статтей на MDN, які частково перекладені на українську мову, також можна вказати посилання на українську версію.

Якщо така стаття немає перекладеної версії, залишайте посилання "як є".

### Метадані

Деякі файли, особливо завдання, мають зверху метадані в форматі YAML, які розділені `---`:

```md
importance: 5

---
...
```

Будь ласка, не перекладайте "importance" (та інші метадані).

## Запуск локально

Ви можете запустити посібник локально, щоб відразу бачити зміни на сайті.
Сервер знаходиться тут: <https://github.com/javascript-tutorial/server>.

---
Будемо дуже вдячні за ваш переклад, або додавання чогось нового!

♥  
Ilya Kantor @iliakan
