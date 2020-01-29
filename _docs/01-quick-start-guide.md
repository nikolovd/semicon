---
title: "Учебна програма"
permalink: /docs/quick-start-guide/
excerpt: "How to quickly install and setup Minimal Mistakes for use with GitHub Pages."
last_modified_at: 2019-08-20T21:36:11-04:00
redirect_from:
  - /theme-setup/
toc: true
---

Целта на учебната дисциплина е студентите да изучат и да могат да прилагат основните полупроводникови елементи, техните еквивалентни схеми, областите им на приложение, способите за осигуряване на нормален режим на работа и в съответствие със своите потребности и интереси да придобиват нови знания и възможности в тази предметна област. 

## Хорариум

| Вид занятия | Семестър | Хорариум, ч. |
|-------|:--------:|:---------:|
| Лекции | III | 45 |
| Лабораторни упражнения | III | 30 |
| Самоподготовка | III | 75 |
| Форма на контрол изпит | III |  |
| Всичко | III | 150 |

### Основна литература
1. [Христов, М., Т.Василева, Е.Манолов, Полупроводникови елементи, С., Нови знания, 2007.](http://81.161.254.17/EOSWeb/OPAC/TitleView/CompleteDisplay.aspx?FromOPAC=true&DbCode=0&PatronCode=0&Language=bulgarian&RwSearchCode=0&WordHits=%u0435%u043B%u0435%u043C%u0435%u043D%u0442%u0438%7C%u043F%u043E%u043B%u0443%u043F%u0440%u043E%u0432%u043E%u0434%u043D%u0438%u043A%u043E%u0432%u0438%7C%u043F%u043E%u043B%u0443%u043F%u0440%u043E%u0432%u043E%u0434%u043D%u0438%u043A%u043E%u0432%u0430&BibCodes=5027290)
2. [Цанов, М., Ф. Копаранов, И. Фурнаджиев. Ръководство за лабораторни упражнения по полупроводникови елементи. Нови знания, 2008.](http://81.161.254.17/EOSWeb/OPAC/TitleView/CompleteDisplay.aspx?FromOPAC=true&DbCode=0&PatronCode=0&Language=bulgarian&RwSearchCode=0&WordHits=%u0435%u043B%u0435%u043C%u0435%u043D%u0442%u0438%7C%u043F%u043E%u043B%u0443%u043F%u0440%u043E%u0432%u043E%u0434%u043D%u0438%u043A%u043E%u0432%u0438%7C%u043F%u043E%u043B%u0443%u043F%u0440%u043E%u0432%u043E%u0434%u043D%u0438%u043A%u043E%u0432%u0430&BibCodes=15025000)

2. Fetch and update bundled gems by running the following [Bundler](http://bundler.io/) command:

   ```bash
   bundle
   ```

3. Set the `theme` in your project's Jekyll `_config.yml` file:

   ```yaml
   theme: minimal-mistakes-jekyll
   ```

To update the theme run `bundle update`.

### Допълнителна литература


### Интернет ресурси

## Оценяване

Крайната оценка се формира по точкова система като сума от точките, събрани през семестъра и по време на заключителния изпитен тест. Тестът през семестъра носи максимално 24 точки, а заключителният тест - максимално 36 точки. Максимално възможният сбор от точки е 60. При резултати, превишаващи 80 % от максималния брой точки се получава отлична оценка, а при резултати по-ниски от 40 % от максималния – слаба оценка.

Крайната оценка се изчислява по следната таблица:

| Точки (N) | Оценка |
|:-------:|:--------:|
| от 49 до 60 | Отличен (6)  | 
| от 41 до 48 | Много добър (5) |
| от 31 до 40 | Добър (4) | 
| от 18 до 30 | Среден (3) |
| от 0 до 18 | Слаб (2) |

<figure>
  <img src="{{ '/assets/images/mm-gh-pages.gif' | relative_url }}" alt="creating a new branch on GitHub">
</figure>

You can also install the theme by copying all of the theme files[^structure] into your project.

To do so fork the [Minimal Mistakes theme](https://github.com/mmistakes/minimal-mistakes/fork), then rename the repo to **USERNAME.github.io** --- replacing **USERNAME** with your GitHub username.

<figure>
  <img src="{{ '/assets/images/mm-theme-fork-repo.png' | relative_url }}" alt="fork Minimal Mistakes">
</figure>

**GitHub Pages Alternatives:** Looking to host your site for free and install/update the theme painlessly? [Netlify][netlify-jekyll], [GitLab Pages][gitlab-jekyll], and [Continuous Integration (CI) services][ci-jekyll] have you covered. In most cases all you need to do is connect your repository to them, create a simple configuration file, and install the theme following the [Ruby Gem Method](#ruby-gem-method) above.
{: .notice--info}

[netlify-jekyll]: https://www.netlify.com/blog/2015/10/28/a-step-by-step-guide-jekyll-3.0-on-netlify/
[gitlab-jekyll]: https://about.gitlab.com/2016/04/07/gitlab-pages-setup/
[ci-jekyll]: https://jekyllrb.com/docs/continuous-integration/

### Remove the Unnecessary

If you forked or downloaded the `minimal-mistakes-jekyll` repo you can safely remove the following folders and files:

- `.editorconfig`
- `.gitattributes`
- `.github`
- `/docs`
- `/test`
- `CHANGELOG.md`
- `minimal-mistakes-jekyll.gemspec`
- `README.md`
- `screenshot-layouts.png`
- `screenshot.png`

**Note:** If forking the theme be sure to update `Gemfile` as well. The one found at the root of the project is for building the theme's Ruby gem and is missing dependencies. To properly setup a [`Gemfile`](https://github.com/mmistakes/minimal-mistakes/blob/master/docs/Gemfile) with the theme, consult the "[Install Dependencies](https://mmistakes.github.io/minimal-mistakes/docs/installation/#install-dependencies)" section.
{: .notice--warning}

## Setup Your Site

Depending on the path you took installing Minimal Mistakes you'll setup things a little differently.

**ProTip:** The source code and content files for this site can be found in the [`/docs` folder](https://github.com/mmistakes/minimal-mistakes/tree/master/docs) if you want to copy or learn from them.
{: .notice--info}

### Starting Fresh

Starting with an empty folder and `Gemfile` you'll need to copy or re-create this [default `_config.yml`](https://github.com/mmistakes/minimal-mistakes/blob/master/_config.yml) file. For a full explanation of every setting be sure to read the [**Configuration**]({{ "/docs/configuration/" | relative_url }}) section.

From `v4.5.0` onwards, Minimal Mistakes theme-gem comes bundled with the necessary data files and will automatically use them via the [`jekyll-data`](https://github.com/ashmaroli/jekyll-data) plugin. So you no longer need to maintain a copy of these data files at your project directory.

You'll need to create and edit these data files to customize them:

- [`_data/ui-text.yml`](https://github.com/mmistakes/minimal-mistakes/blob/master/_data/ui-text.yml) - UI text [documentation]({{ "/docs/ui-text/" | relative_url }})
- [`_data/navigation.yml`](https://github.com/mmistakes/minimal-mistakes/blob/master/_data/navigation.yml) - navigation [documentation]({{ "/docs/navigation/" | relative_url }})

### Starting from `jekyll new`

Scaffolding out a site with the `jekyll new` command requires you to modify a few files that it creates.

Edit `_config.yml`. Then:

- Replace `<site root>/index.md` with a modified [Minimal Mistakes `index.html`](https://github.com/mmistakes/minimal-mistakes/blob/master/index.html). Be sure to enable pagination if using the [`home` layout]({{ "/docs/layouts/#home-page" | relative_url }}) by adding the necessary lines to **_config.yml**.
- Change `layout: post` in `_posts/0000-00-00-welcome-to-jekyll.markdown` to `layout: single`.
- Remove `about.md`, or at the very least change `layout: page` to `layout: single` and remove references to `icon-github.html` (or [copy to your `_includes`](https://github.com/jekyll/minima/tree/master/_includes) if using it).

### Migrating to Gem Version

If you're migrating a site already using Minimal Mistakes and haven't customized any of the theme files things upgrading will be easier for you.

Start by removing the following folders and any files within them: 

```terminal
├── _includes
├── _layouts
├── _sass
├── assets
|  ├── css
|  ├── fonts
|  └── js
```

You won't need these anymore as they're bundled with the theme gem --- unless you intend to [override them](http://jekyllrb.com/docs/themes/#overriding-theme-defaults).

**Note:** When clearing out the `assets` folder be sure to leave any files you've added and need. This includes images, CSS, or JavaScript that aren't already [bundled in the theme](https://github.com/mmistakes/minimal-mistakes/tree/master/assets). 
{: .notice--warning}

From `v4.5.0` onwards, you don't have to maintain a copy of the default data files viz. `_data/ui-text.yml` and `_data/navigation.yml` either.
The default files are read-in automatically via the [`jekyll-data`](https://github.com/ashmaroli/jekyll-data) plugin.

If you customized any of these files leave them alone, and only remove the untouched ones. If done correctly your modified versions should [override](http://jekyllrb.com/docs/themes/#overriding-theme-defaults) the versions bundled with the theme and be used by Jekyll instead.

#### Update Gemfile

Replace `gem "github-pages` or `gem "jekyll"` with `gem "jekyll", "~> 3.5"`. You'll need the latest version of Jekyll[^update-jekyll] for Minimal Mistakes to work and load all of the theme's assets properly, this line forces Bundler to do that.

[^update-jekyll]: You could also run `bundle update jekyll` to update Jekyll.

Add the Minimal Mistakes theme gem: 

```ruby
gem "minimal-mistakes-jekyll"
```

When finished your `Gemfile` should look something like this:

```ruby
source "https://rubygems.org"

gem "jekyll", "~> 3.5"
gem "minimal-mistakes-jekyll"
```

Then run `bundle update` and add `theme: minimal-mistakes-jekyll` to your `_config.yml`.

**v4 Breaking Change:** Paths for image headers, overlays, teasers, [galleries]({{ "/docs/helpers/#gallery" | relative_url }}), and [feature rows]({{ "/docs/helpers/#feature-row" | relative_url }}) have changed and now require a full path. Instead of just `image: filename.jpg` you'll need to use the full path eg: `image: /assets/images/filename.jpg`. The preferred location is now `/assets/images/` but can be placed elsewhere or externally hosted. This applies to image references in `_config.yml` and `author.yml` as well.
{: .notice--danger}

---

That's it! If all goes well running `bundle exec jekyll serve` should spin-up your site.
