# Инструкция для работы Markdown

## Введение

Начинаем работу в Markdown

## Заголовки

Для того чтобы выделить заголовок, необходимо поставить от 1 до 6 решёток (#) и пробел в самом начале строки. 

Уровень заголовка зависит только от количества решёток.

(#) пробел - заголовок 1 уровня

(##) пробел - заголовок 2 уровня

(###) пробел заголовок 3 уровня

И так далее.

## Выделение текста

Если обернуть текст звёздочками (*) , то он станет жирным или курсивным. 

Стиль выделения зависит только от их количества.

Пример:

* одна пара * сделает текст курсивным;

* две пары * сделают текст жирным;

* три пары * применят оба стиля.

Получим вид:

Обычный текст

*Курсивный текст*

**Жирный текст**

***Оба стиля***

**Зачеркивание**

Если необходимо зачеркнуть текст, то можно поставить по две тильды (~~) в начале и в конце фрагмента.

Пример:

~ ~ Привет, Вова!~ ~ (без пробела)

Здравствуйте, Владимир!

Получим:

~~Привет, Вова!~~\
Здравствуйте, Владимир!

## Списки

Для создания маркированных (ненумерованных) списков перед каждым пунктом нужно поставить минус (-), плюс (+) или звёздочку (*). Маркер и текст пункта необходимо разделять пробелом.

(-) Помидор

(-) Огурец

(+) Бублик

(+) Ватрушка

(*) Молоко

(*) Кефир

Если перед подряд идущими пунктами будут стоять разные маркеры, то после конвертации мы получим разные списки.

Получим:

- Помидор
- Огурец

+ Бублик
+ Ватрушка

* Молоко
* Кефир

***Упорядочные***

Если в качестве маркеров использовать цифры c точкой на конце (1., 2. и т. д.), то мы получим упорядоченный (нумерованный) список.

Пример:

(1.) Хлеб

(2.) Молоко

(3.) Помидоры

Получим:

1. Хлеб
2. Молоко
3. Помидоры

***Вложенность***

Любые списки можно вкладывать друг в друга, для этого перед маркером нужно поставить таб или несколько пробелов.

Пример:

(+) Хлеб

(+) Молочные продукты

(1.) Кефир

(2.) Ряженка

(1.) Молоко

(2.) Хлебобулочные изделия

(+) Бублик

(+) Ватрушка

Получим:

+ Хлеб
+ Молочные продукты
  1. Кефир
  2. Ряженка

1. Молоко
2. Хлебобулочные изделия
    + Бублик
    + Ватрушка
    
## Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее:

![Привет, цветочек!](%D0%A6%D0%B2%D0%B5%D1%82%D0%BE%D1%87%D0%B5%D0%BA.png)

## Ссылки

Markdown предлагает 3 стиля разметки ссылок: *строчный, справочный и автоматический*.

***Строчные***

Для вставки ссылки в строчном стиле необходимо воспользоваться следующей конструкцией: 
[Текст ссылки](URL). 

Есть возможность добавить подсказку, для этого нужно после URL дописать текст в кавычках: [Текст ссылки](URL "Подсказка").

***Справочные*** 

Для вставки ссылки в справочном стиле нужно написать 

[Текст ссылки][Ключ] в том месте, где вы хотите её поместить, а где-нибудь выше или ниже добавить сноску [Ключ]: URL "Подсказка".

***Автоматические***

Markdown позволяет использовать упрощённый вариант для вставки ссылок, для этого нужно просто обернуть URI треугольными скобками (<URI>).

Так же можно вставлять адреса электронной почты (<hi@doka.guide>).

## Работа с таблицами

Колонки таблицы размечаются с помощью вертикальных черт (|), а заголовок отделяется дефисами (-).

Пример:

(|) Место (|) Участник (|)Рейтинг (|)

(|-------|----------|---------|)

(| 1     | Саша     | 118     |)

(| 2     | Юля      | 92      |)

(| 3     | Даниил   | 36      |)

Получим вид:

| Место | Участник | Рейтинг |
|-------|----------|---------|
| 1     | Саша     | 118     |
| 2     | Юля      | 92      |
| 3     | Даниил   | 36      |

## Цитаты

    Если в начале строки поставить треугольную скобку (>), то Markdown превратит текст после неё в цитату. 
    
    Внутри могут быть любые блоки: параграфы, заголовки или даже другие цитаты.

    Пример:

(> ( *** ) ) Цитаты великих людей (***)

(>) Ваша работа заполнит большую часть жизни и единственный способ быть

(>) полностью довольным — делать то, что по-вашему является великим делом.

(>) И единственный способ делать великие дела — любить то, что вы делаете.
(>)

(> *—) Стив Джобс, Речь в Стенфорде*

Получим:

> ***Цитаты великих людей***

> Ваша работа заполнит большую часть жизни и единственный способ быть
> полностью довольным — делать то, что по-вашему является великим делом.
> И единственный способ делать великие дела — любить то, что вы делаете.
>
> *— Стив Джобс, Речь в Стенфорде*

# **Работа с удаленными репозитариями**

Коммит, созданный нами, хранится в репозитарии, привязанном к конкретной папке на нашем компьютере, т.е. является локальным. Это полезно, если мы работаем над проектом самостоятельно. Однако в большинстве случаев возникает необходимость обеспечить доступ к результатам работы или доставить код на сервер, где он будет выполняться.

Для загрузки данных в удаленный репозитарию сначала нужно к нему подключиться, однако пользователь может создать собственный удаленный репозитарий на GitHub. Это занимает некоторое время, однако в дальнейшем полностью себя оправдывает, тем более, что подобные службы имеют пошаговые инструкции для правильно выполнения нужных действий.

Иногда бывает так, что проект имеет несколько удаленных репозитариев – в таком случае каждому из них присваивается собственное имя. Главный репозитарий принято называть origin.

## Основные команды ##

***git clone <ссылка на удаленный репозиторий>***

Клонирует переданный репозиторий на ваш компьютер.

***git fetch [ключи] [имя удаленного репозитория]***

Получает изменения из переданного удаленного репозитория. Если не было передано ни одного удаленного репозитория, ни ключа --all, команда пытается получить изменения из репозитория с именем origin.

***git pull [ключи] [имя удаленного репозитория]***

Получает изменения из переданного удаленного репозитория и обновляет рабочую копию в соответствии с удаленным репозиторием. По умолчанию слияние удаленной ветки с локальной происходит именно в fast-forward режиме, так что включать его специально не требуется

***git push [ключи] [имя удаленного репозитория] [имя ветки]***

Загружает изменения в удаленный репозиторий. Если слияние изменений в удаленном репозитории нельзя сделать в режиме fast-forward, и при этом не был передан ключ force, выполнение закончится с ошибкой.

***git remote***

Команда git remote служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные репозиториев в виде понятных коротких строк, например «origin», так что вам не придётся забивать голову всякой ерундой и набирать её каждый раз для связи с сервером. Вы можете использовать несколько удалённых репозиториев для работы и git remote поможет добавлять, изменять и удалять их.

***git archive***

Команда git archive используется для упаковки в архив указанных коммитов или всего репозитория.

***git submodule***

Команда git submodule используется для управления вложенными репозиториями. Например, это могут быть библиотеки или другие, используемые не только в этом проекте ресурсы.

**Вывод**

Таким образом, вы можете вносить свой вклад в абсолютно любые приложения с открытым программным кодом. Даже репозиторий самого Git хранится на GitHub, и вы в любой момент можете сделать форк и придумать новую команду (правда не факт, что ответственный примет ваш пулл-реквест). Вы можете внести свой вклад в разработку ядра Linux, в популярный редактор Visual Studio Code, в ядро криптовалюты Bitcoin, в языки программирования Python, Go, Ruby – все эти проекты имеют открытые репозитории на GitHub.

## Заключение

# **Удачного обучения!!!**