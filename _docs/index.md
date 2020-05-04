---
title: Приступим
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Начало

[GitHub Pages](https://pages.github.com) могут автоматически сгенерировать
и предоставить размешение для вашего сайта.  Допустим у вас есть username/organisation 
`my-org` и проект `my-proj`; Если вы расположите код Jekyll в папке `docs` в ветке 
master вашего репозитория `github.com/my-org/my-proj`, то сайт будет размещён по адресу 
`my-org.github.io/my-proj`. Идея соединения вашей документации с
репозиторием исходного кода состоит в том что всякий раз когда вы добавляете
новую информацию по какому то функционалу в основной ветке, она так же будет
немедленно опубликована на веб-странице.

1. Просто [добавьте содержимое](https://github.com/aksakalli/jekyll-doc-theme/archive/gh-pages.zip) в папку `docs` вашего репозитория.
2. Отредактируйте настройки сайта в файле `_config.yml` в соответствии с вашим проектом. !!! `baseurl` доржен быть относительным URI вашего сайта, как`/my-proj` !!!
3. Замените `favicon.ico` и `assets/img/logonav.png` своими логотипами.

## Наполнение контентом

### Документация 

Документация это [коллекция](https://jekyllrb.com/docs/collections/) страниц хранящихся в папке `_docs`. 
Для создания новой страницы:

**1.** Create a new Markdown as `_docs/my-page.md` and write [front matter](https://jekyllrb.com/docs/frontmatter/) & content such as:

```
---
title: My Page
permalink: /docs/my-page/
---

Hello World!
```

**2.** Add the pagename to `_data/docs.yml` file in order to list in docs navigation panel:

```
- title: My Group Title
  docs:
  - my-page
```

### Blog posts

Add a new Markdown file such as `2017-05-09-my-post.md` and write the content similar to other post examples.

### Pages

The homepage is located under `index.html` file. You can change the content or design completely different welcome page for your taste. (You can use [bootstrap components](http://getbootstrap.com/components/))

In order to add a new page, create a new `.html` or `.md` (markdown) file under root directory and link it in `_includes/topnav.html`.
