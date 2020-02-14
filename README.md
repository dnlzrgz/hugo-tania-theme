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
copyright = ""
```

### Contact

To add your contact email to the footer you'll need to add to your `config.toml` the following lines:

```toml
[params.contact]
  email = "you@email.com"
```

### Social

To add your social links to the footer you'll need to add:

```toml
[params.social]
  codepen = "codepen.io/yourusername"
  github = "github.com/yourusername"
  linkedin = "linkedin.com/in/yourprofile"
  twitter = "twitter.com/yourusername"
```

But the above is just an example, you can add any link you want and it will be rendered as follows:

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

## Things I'm working on

- Blogging support.
- Better customization to change easily things like the color scheme.
- Dark mode.
- Caching with Service Workers.
- Better lists pages.