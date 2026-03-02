# GitHub Pages Blog Starter

This repository is a starter for a personal `github.io` blog with sections for:
- Technical news
- Ideas
- Experience
- CV
- Post comments (optional via Giscus)

## 1) Create your GitHub Pages repository

For a user site, the repository name must be:
- `soohwan.github.io`

Then push this project there.

## 2) Update site settings

Edit [`_config.yml`](./_config.yml):
- `title`
- `description`
- `url` (set to your final Pages URL)
- `author`

## 3) Write content

- Blog posts: [`_posts/`](./_posts)
- Experience page: [`experience.md`](./experience.md)
- CV page: [`cv.md`](./cv.md)
- About page: [`about.md`](./about.md)

## 4) Enable comments (optional)

This starter uses [Giscus](https://giscus.app/).

1. Enable **GitHub Discussions** in your repository.
2. Go to Giscus and generate your `repo_id` and `category_id`.
3. Update `giscus` values in `_config.yml`.
4. Set `giscus.enabled: true`.

## 5) Local preview (optional)

If you have Ruby/Jekyll installed:

```bash
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

## Publishing

On the `soohwan.github.io` repository, GitHub Pages publishes from the default branch root by default.
