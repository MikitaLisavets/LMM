
LMM Методология
===============
> ***layout module modificator***

> Принципом методологии является максимальная модульность, независимость
> и переиспользование блоков верстки.

 - [Методология] (#structure)
 - [Javascript Plugins] (#plugins)
 - [Sublime text packages] (#sublime)

Structure:
---------

  - Базовый слой (base)
  - Слой разметки (layout)
  - Слой модулей (module)
  - Модификации

![](https://dl.dropboxusercontent.com/u/80313909/github/flat.png)

Base
----
  Основные правила для этого слоя:
  - сбросы стилей ( normalize, reset, etc. );
  - конфигураци, миксины, функции, переменные sass и compass
  - стили для общих элементов без классов и id ( html, body, a, ul, etc. );

![](https://dl.dropboxusercontent.com/u/80313909/github/base.png)


Layout
------
  Основные правила для этого слоя:
  - стили для общей разметки и сетки страницы ( .l-header, .l-col_12, .l-aside,
      etc. ).
  - классы начинаются с префикса ".l-";

![](https://dl.dropboxusercontent.com/u/80313909/github/layout.png)



Module
------

  Основные правила для этого слоя:
  - стили для абсолютно независимых блоков, которые могу в себе содержать другие модули и подмодули;
  - классы начинаются с префикса ".m-";
  - имя модуля состоящего из более чем 1-го слова разделяются
      символом тире "-" ( .m-reg-form, .m-shopping-cart, etc. );

![](https://dl.dropboxusercontent.com/u/80313909/github/module.png)


Sub-module
---------

  - имя подмодуля составляется из имени модуля + символ нижнего подчеркивания "_" + имя подмодуля (.m-form_item)

![](https://dl.dropboxusercontent.com/u/80313909/github/component.png)


Modification
------------

  - добавляет дополнительные свойства для общих элементов layout и module
  - классы начинаются с префикса ".__";


![](https://dl.dropboxusercontent.com/u/80313909/github/all.png)




Plugins:
------------------------------------

```sh

[
  {
    category: "Стилизация форм",
    listPlugins: [
      {
        title: "jQueryFormStyler",
        link: "https://github.com/Dimox/jQueryFormStyler",
        description: ""
      }
    ]
  },
  {
    category: "Кастомизация скролла",
    listPlugins: [
      {
        title: "Nicescroll",
        link: "https://github.com/inuyaksa/jquery.nicescroll",
        description: ""
      }
    ]
  },
  {
    category: "Скролл эффекты",
    listPlugins: [
      {
        title: "Scroolly",
        link: "https://github.com/chayka/jQuery.Scroolly",
        description: ""
      }
    ]
  },
  {
    category: "Датапикеры",
    listPlugins: [
      {
        title: "Pikaday",
        link: "https://github.com/dbushell/Pikaday",
        description: ""
      },
      {
        title: "Pikadate",
        link: "https://github.com/amsul/pickadate.js",
        description: "ie9+"
      }
    ]
  },
  {
    category: "Слайдеры",
    listPlugins: [
      {
        title: "Swiper",
        link: "https://github.com/nolimits4web/Swiper",
        description: ""
      }
    ]
  },
  {
    category: "Рейтинги",
    listPlugins: [
      {
        title: "Raty",
        link: "https://github.com/wbotelhos/raty",
        description: ""
      }
    ]
  }
]


```
