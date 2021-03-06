
> This is a rework of **theseanstewart/Gitbook-Plugin-Image-Wrapper**, which extends ability to have different class on each page.


# Gitbook Custom Image Class Plugin

This plugin will wrap your images in a div with a class of *image-wrapper*. This allows you to add CSS styles to style the way the image is displayed.

```
<div class="image-wrapper" />
```

## Usage

### Installation

Add the plugin to your `book.json`:

```
{
    "plugins" : [ "image-class" ]
}
```

### Add Images

For example, in `introduction.md` file, add images normally to your document using Markdown

```
![Alt Text](/assets/image-url.jpg)
```

Each image will be wrapped in a div like this 

```
<div class="image-wrapper introduction">
	<img src="/assets/image-url.jpg" alt="Alt Text" />
</div>
```

### Style It

Add the following CSS to your book to center your images and add some additional spacing:

```
.image-wrapper.introduction {
	text-align: center;
	padding: 15px 0px;
}
```

## Why

When building documentation for my business [AppStorm](https://appstorm.co), I wondered whether I can customized image size, on each different page. I came accross [theseanstewart/Gitbook-Plugin-Image-Wrapper](https://github.com/theseanstewart/Gitbook-Plugin-Image-Wrapper) repository and thought that I could improve it better. So I reworked a little bit so it will support.

<a target='_blank' rel='nofollow' href='https://app.codesponsor.io/link/kJbeTd1SaSwKTLd6NYQ1MuSr/appstormco/gitbook-plugin-image-class'>  <img alt='Sponsor' width='888' height='68' src='https://app.codesponsor.io/embed/kJbeTd1SaSwKTLd6NYQ1MuSr/appstormco/gitbook-plugin-image-class.svg' /></a>
