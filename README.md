# Responsividade 

Criando um site responsivo com layouts flexiveis de acordo com o dispositivo acessado. Sendo ele smartphone, tablet ou desktop. E até mesmo uma impressora.

Usando estratégias de CSS Units para que tanto o nosso Layout, quanto os nossos textos, fiquem fluidos. 

Utilizaremos também CSS Media Queries para adicionar CSS customizados conforme o breakpoint definido, para que nosso layout fique adaptado ao viewport do dispositivo. 


## Resources

- [x] HTML5, CSS3, JS
- [x] SVG Images


Notas importantes! 📝


## CSS Units

Unidades de medidas do CSS

Layout Fixo
`px` - Pixels

Layout Fluido
`%` - Porcentagem
`auto` - Automática
`vh` - Viewport Height
`vw` - Viewport Width

Textos fixos
`1px` = 0.75pt
`16px` = 12pt

Texto fluidos
`em` - multiplicado pelo pai 
`rem` - multiplicado pelo root


## CSS Media Queries 

No HTMl colocar a seguinte tag meta

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

No CSS usar da seguinte forma

```css
@media (max-width: 320px) {
  #form h3 {
    font-size: 2rem;
  }
}
```


## HTML Media Attrib.

Utilizar o atribuito `media` no link do meu HTML, ao importar um arquivo css, usando as propriedades da mesma forma que usaria na regra `@media` do css.

```html
<link 
    rel="stylesheet"
    href="responsive.css" 
    media="screen and (max-width: 768px)"
/>

<link rel="stylesheet" href="print.css" media="print">
```


## Imagens

Usar a tag `<picture>` para que as imagens sejam responsivas.

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
Sempre que possível, usar SVG ao invés de JPG, PNG.


### Desktop | Mobile:
![webpage](https://imgur.com/gallery/9tv4FRg.png)
