# Responsiveness

Creating a responsive website with flexible layouts according to the device accessed. Whether it's smartphone, tablet or desktop. And even a printer.

Using CSS Units strategies so that both our Layout and our texts are fluid.

We will also use CSS Media Queries to add custom CSS according to the defined breakpoint, so that our layout is adapted to the device's viewport.


## Resources

- [x] HTML5, CSS3, JS
- [x] SVG Images


Important notes!📝


## CSS Units

CSS measurement units

Fixed Layout
`px` - Pixels

Fluid Layout
`%` - Percentage
`auto` - Automatic
`vh` - Viewport Height
`vw` - Viewport Width

Fixed texts
`1px` = 0.75pt
`16px` = 12pt

fluid text
`in` - multiplied by the parent
`rem` - multiplied by root

## CSS Media Queries

In HTMl put the following meta tag

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

In CSS use as follows
```css
@media (max-width: 320px) {
  #form h3 {
    font-size: 2rem;
  }
}
```


## HTML Media Attrib.

Use the `media` attribute in my HTML link, when importing a css file, using the properties the same way you would in the `@media` css rule.
```html
<link 
    rel="stylesheet"
    href="responsive.css" 
    media="screen and (max-width: 768px)"
/>

<link rel="stylesheet" href="print.css" media="print">
```


## Images

Use the `<picture>` tag to make images responsive.

```html
<picture class="image" alt="Imagem">
    <source media="(min-width: 768px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/maxresdefault.jpg">
    <source media="(min-width: 320px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg">
    <source media="(min-width: 10px)" 
        srcset="https://i.ytimg.com/vi/GykTLqODQuU/mqdefault.jpg">

    <img 
        src="https://i.ytimg.com/vi/GykTLqODQuU/hqdefault.jpg" 
        alt="Imagem" />
</picture>
```
Whenever possible, use SVG instead of JPG, PNG.

