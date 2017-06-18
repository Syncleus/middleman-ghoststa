# middleman-ghoststa

## Installation

1. Create a new project with the template:

  ```bash
  middleman init -T Syncleus/middleman-ghoststa MY_PROJECT_FOLDER
  ```

2. Change the `ghoststa` settings in `config.rb`.

## Usage

Start a local web server running at `http://localhost:4567/` with:

```bash
bundle exec middleman server
```

Create a static file with:

```bash
bundle exec middleman build
```

For help, see the official [Middleman](https://middlemanapp.com) website.

### Author

Configurable in *config.rb*:

```ruby
config[:ghoststa] = {
  ...
  author: {
    name: 'Middleman'
  }
  ...
}
```

### Navigation

Configurable in *config.rb*:

```ruby
config[:ghoststa] = {
  ...
  navigation: {
    "Home" => "/",
    "GitHub" => "https://github.com",
    "Author" => "/author/middleman/"
  }
  ...
}
```

### Logo

Configurable in *config.rb*:

```ruby
config[:ghoststa] = {
  ...
  blog: {
    logo: 'my-awesome-blog-logo.png' # sources/images/my-awesome-blog-logo.png
  }
  ...
}
```

### Pages

Content of *example.html.markdown*:

```markdown
---
title: Example
layout: page
---

Welcome!
```

### Covers

Covers are availible in pages and articles. Content of *example.html.markdown*:

```markdown
---
title: Example
layout: page
cover: my-awesome-blog-cover.png # sources/images/my-awesome-blog-cover.png
---

Welcome!
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new [Pull Request](../../pull/new/master)
