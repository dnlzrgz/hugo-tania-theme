# Tania - A simple and clean theme for Hugo.

## Features

- **Fast**: All the CSS used, once compressed, doesn't reach the 4kb.
- **Simple**: Say what you want without unnecessary decorations.
- **Responsive**: Looks good on all screen sizes.

## Installation

You can install Tania running the following commands inside your Hugo project:

```bash
mkdir themes
cd themes
git clone https://github.com/danielkvist/hugo-tania-theme.git tania
```

Or

```bash
mkdir themes
cd themes
git submudole add https://github.com/danielkvist/hugo-tania-theme.git tania
```

> If you are planning to use Netlify is recommended to install the theme as a git submodule.

Then, on your `config.toml` file change the following line:

```toml
theme = "tania"
```

## Configuration

### Base params

```toml
baseURL = "/"
title = "Your Project Name"
author = "Author"
description = "Descrption of your project."
googleAnalytics = "YOUR-GOOGLE-ANALYTICS-TOKEN"
enableRobotsTXT = true
language = "en-US"
copyright = "© 2020 Daniel (Danielkvist)."
```

### Pagination

To set the number of items per page:

```toml
paginate = 7
```

### Code

To use the CSS styles defined to code blocks you will need to add the following line to your `config.toml` file:

```toml
pygmentsUseClasses=true
```

### Other important params

```toml
[params]
  author = "Your name"
  description = "Tania is a simple and clean theme for Hugo".
  dateFormat = "Monday, Jan 2, 2006"
```

> The parameters above are important and you should ensure that they are defined in your `config.toml` for the correct functioning of Tania.

### Contact

To add your contact email to the footer you'll need to add to your `config.toml` the following lines:

```toml
[params.contact]
  email = "you@email.com"
```

### Social

To add a message before your social links:

```toml
[params.social]
  text = "Find more about me here:"
```

To add your social links to the footer you'll need to add:

```toml
[params.links]
  codepen = "codepen.io/yourusername"
  github = "github.com/yourusername"
  linkedin = "linkedin.com/in/yourprofile"
  twitter = "twitter.com/yourusername"
```

You can add any link you want and it will be rendered as follows:

```html
<!-- Using GitHub as an example -->
<a
  class="..."
  href="github.com/yourusername"
  alt="github"
  target="_blank"
  rel="nofollow"
  >github</a
>
```

## Front Matter

### Single pages without tags

```md
---
title: "About"
description: "What is Tania and why you should care about it"
menu: main
weight: 1
---
```

### Singles pages with tags

```md
---
title: "Golang"
description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin vel nisi massa."
date: 2020-02-17T22:20:00+01:00
publishDate: 2020-02-19T22:20:00+01:00
tags: ["golang", "programming"]
---
```

### List pages

```md
---
title: "Blog"
description: "I'm writing about stuff. Really interesting stuff"
menu: main
weight: 2
---
```

## Things I'm working on

- Better customization to change easily things like the color scheme.
- Dark mode.
- Caching with Service Workers.
