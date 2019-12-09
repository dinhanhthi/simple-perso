---
layout: post
title: "How to modify this theme?"
subtitle: Make this theme be yours
tags: [others]
categories: others
icon-photo: modify.png
date: 2019-06-11
---

{% include toc.html %}

## Your personal info

Open file `_data/me.yml` and modify (you don't have to give all infos):

- `name`: your name, e.g. *Anh-Thi DINH*.
- `shor_name`: your short name (forename), e.g. *Thi*.
- `email`: your email, e.g. *dinhanhthi@gmail.com*.
- `tel`: your telephone number.
- `avatar`: your avatar's url. For example, `img/avatar.png` means that a file called `avatar.png` is placed at `/img/` folder.
- `facebook`: your facebook username, e.g. *math2it*.
- `index-intro`: a bref discription about you. You have put the content between `""`.
- `cv`: your Curriculum Vitae file's url. You can place your file in folder `/files/`.
- `favicon`: the small photo standing on the left of your website in a tab of Chrome.
- `location`: your current location.

## Index page

You can modify file `index.html`.

### Find me on ([check]({{site.url}}{{site.baseurl}}/#social){:target="_blank"})

Modify file `_data/social.yml`:

- `name`: name of the platform.
- `icon`: an icon for this platform. You should use black & white icon (with transparent background). The photo should be placed in `/img/social/`
- `url`: your profile url on this platform.
- `opacity`: if you want the icon be lighter.

### My learning log ([check]({{site.url}}{{site.baseurl}}/my-learning-log){:target="_blank"})

Modify file `pages/my-learning-log.md`.

- `{:.finish}`: for the finished tasks.
- `{:.ongoing}`: for the ongoing tasks.
- `{:.delay}`: for the delayed tasks.
- `{:.fail}`: for interrupted tasks.

For the badges:

- `<span class="tbadge badge-orange">Orange badges</span>`.
- `<span class="tbadge badge-yellow">Yellow badges</span>`.
- `<span class="tbadge badge-green">Green badges</span>`.
- `<span class="tbadge badge-blue">Blue badges</span>`.
- `<span class="tbadge badge-gray">Gray badges</span>`.

### Recent projects ([check]({{site.url}}{{site.baseurl}}/project){:target="_blank"})

Modify file `_data/project.yml` (all the fields should be placed inside quotation marks `""`). List of projects are showed in `/project` (file `/pages/project.md`) and on the index page.

- `title`: project's name.
- `description`: project's description.
- `source`: project's souce code's url.
- `url`: project's website.

💡 **Tip**: the list of projects can be put any where with the shortcut `{% raw %}{% include list_project.html limit=5 %}{% endraw %}` (remove `limit=5` if you wanna show all the projects).

### Recent read books ([check]({{site.url}}{{site.baseurl}}/reading){:target="_blank"})

Modify file `_data/book.yml` (all the fields should be placed inside quotation marks `""`). List of books are showed in `/reading` (file `/pages/reading.md`) and on the index page.

- `title`: book's name.
- `intro`: book's introduction.
- `author`: book's author.
- `goodreads`: the link to your review for this book on goodreads. If you don't have any review, you can put the book url on goodreads.
- `reading`: `true` if you are reading this book. If you have already read it, don't use this field!
- `mychoice`: `1` if you really like this book!

💡 **Tip**: the list of books can be put any where with the shortcut `{% raw %}{% include list_reading.html limit=5 %}{% endraw %}` (remove `limit=5` if you wanna show all the books).

### Blog posts ([check]({{site.url}}{{site.baseurl}}/blog){:target="_blank"})

All the blog posts must be placed in folder `_posts/` and their name should be in the form of `YYYY-MM-DD-name-of-the-post.md` (You have to use [markdown](https://markdown-it.github.io/) to write the posts). List of posts are showed in `/blog` (file `/pages/blog.md`) and on the index page.

At the beginning of each post, you should indicate some information

~~~{%raw%}
---
layout: post
title: "How to modify this theme?"
subtitle: Make this theme be yours
tags: [others]
categories: others
---
{%endraw%}~~~

💡 **Tip**: the list of posts can be put any where with the shortcut `{% raw %}{% include list_post.html limit=5 %}{% endraw %}` (remove `limit=5` if you wanna show all the posts).

### Note taking ([check]({{site.url}}{{site.baseurl}}/#mynote){:target="_blank"})

Modify file `index.html` (at section `Notes`).

### Personal Sketches ([check]({{site.url}}{{site.baseurl}}/#drawing){:target="_blank"})

Modify file `index.html` (at section `Drawing`) and file `_data/drawing.yml`. The photos should be placed in `/img/sketch/`. For each photo, you should have 2 versions: `new1.jpg` and `new1_thumbnail.jpg` (the `_thumbnail` version is used for the first loading, it should have small size.)

## Others

You can read [this post]({{site.url}}{{site.baseurl}}/how-to-use) for other aspects.