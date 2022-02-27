# Introducing Hit Counter for Your GitHub or Any Kind of Websites You Want

![Hits.sh](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rwaij8wthlz6n721udgh.png)

## What is Hits?
`Hits` is a simple and easy to use web application that counts the number of hits on your website.

If you're familiar with GitHub, you've probably already seen hit counter in the documentation on the GitHub repository:

[![Hits](https://hits.sh/github.com/silentsoft/hits.svg)](https://hits.sh/github.com/silentsoft/hits/)

## Getting Started
`Hits` supports the following three of the most common use cases: `Markdown`, `HTML` and `Image Link`.

For example, to get a hits badge for `https://github.com/silentsoft/hits`:

- Markdown
  ```markdown
  [![Hits](https://hits.sh/github.com/silentsoft/hits.svg)](https://hits.sh/github.com/silentsoft/hits/)
  ```
- HTML
  ```html
  <a href="https://hits.sh/github.com/silentsoft/hits/"><img alt="Hits" src="https://hits.sh/github.com/silentsoft/hits.svg"/></a>
  ```
- Image Link
  ```
  https://hits.sh/github.com/silentsoft/hits.svg
  ```

## Features in Query String

### view
- `total` (default)
- `today-total`

### style
- `flat` (default)
- `flat-square`
- `for-the-badge`
- `plastic`

### label
- For setting the label text instead of the default `hits`.

### extraCount
- This is useful if you want to add an extra count to your badge. For example, if you want to add a count of `1000` to your badge, you can set `extraCount=1000`.
- **When Do I Need This?**
    - If the hit counter service you used previously has end-of-service, you can start with any number instead of starting from 1.

### color, labelColor
- Named color by [shields.io](https://shields.io/)
- Any valid [CSS color](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)
    - named color
    - hexadecimal numbers
    - `rgb[a](red, green, blue[, opacity])`
    - `cmyk[a](cyan, magenta, yellow, black[, opacity])`
    - `hsl[a](hue, saturation, lightness[, opacity])`

### logo
- [simple-icons slug](https://github.com/simple-icons/simple-icons/blob/develop/slugs.md)
- or data:image/svg+xml;base64,..

## Statistics
You can see the statistics of your website by replacing the `.svg` with `/` in the URL you used to get the badge.

For example, to get a statistics for `https://github.com/silentsoft/hits` then visit [https://hits.sh/github.com/silentsoft/hits/](https://hits.sh/github.com/silentsoft/hits/)

![Hits Statistics](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/97l2lcm4u7g8ynsaro9v.png)

## Conclusion

`Hits` is a simple, easy to use, and free to use hit counter badge for your website.

Thank you for reading this article. If you like `Hits`, give it a :star2: on [GitHub](https://github.com/silentsoft/hits).

{% github silentsoft/hits %}