# CSS Naming Conventions

A collection of common CSS naming conventions based on Components, Subcomponents, and Modifiers. 

Over the last few years I've really enjoyed seeing the evolution of [HTML semantics & front-end architecture](http://nicolasgallagher.com/about-html-semantics-front-end-architecture/) and how it's introduced clever methodologies that make CSS more readable, scaleable, and intuitive. I've really enjoyed implementing and learning about [Object Oriented CSS](https://github.com/stubbornella/oocss/wiki), [SMACSS](http://smacss.com) by [Johnathan Snook](https://twitter.com/snookca), and the [BEM Methodology](http://bem.info/) by Yandex. 

While learning from these approaches and [using them in my projects](https://css-tricks.com/design-systems-building-future/) I realized that naming things is easily one of the most frustrating parts of development. In an effort to make it easier on myself and others who feel the same, I've put together a list of common CSS naming conventions that utilize the methodologies mentioned above. Feel free to fork, remix, and do as you please. 

---

## The Naming Convention

My prefered naming conventions follows the [SUIT CSS naming conventions](https://github.com/suitcss/suit/blob/master/doc/naming-conventions.md) very closely:

```
/* Components */
.myComponent {}                     /* Components - camelCase component name */
.myComponent--modifier {}           /* Modifiers - Two dashes for the modifier */
  .myComponent-subComponent {}      /* Subcomponent - One dash for the subcomponent */

/* States */
.myComponent.is-active {}           /* State classes are chained */

/* Objects */
.o-myObject {}                      /* Object classes are prefixed with `o-` */

/* Utils */
.u-myHelper {}                      /* Utility classes are prefixed with `u-` */

/* Javascript Hooks */
.js-myComponent {}                  /* JavaScript classes are prefixed with `js-` and ONLY used as a JS hook */

```


## Native HTML Elements

```
.heading
.heading--h1
.heading--h2
.heading--h3
.heading--h4
.heading--h5
.heading--h6

.link
.link--alt

.list
  .list-item
.list--bare

.form
  .form-fields
  .form-field
  .form-actions
.form--inline
.form--search

.input
.input--checkbox
.input--radio
.input--select
.input--text
.input--file
.input--email
.input--url

.img
.img--responsive
.img--responsiveFill
.img--round
.img--bordered

.table
  .table-head
  .table-foot
  .table-th
  .table-tr
  .table-td
.table--striped
.table--bordered

.btn
.btn--default
.btn--primary
.btn--secondary
.btn--pill
.btn--soft
.btn--hard
```

## Custom Components
```
.alert
  .alert-close
  .alert-header
  .alert-body
  .alert-footer
.alert--success
.alert--info
.alert--warning
.alert--error

.accordion
  .accordion-panel
    .accordion-panel-trigger
    .accordion-panel-content
.accordion--vertical
.accordion--horizontal

.carousel
  .carousel-item
  .carousel-controls
  
.dropdown
  .dropdown-trigger
  .dropdown-content

.flexEmbed
  .flexEmbed-ratio
  .flexEmbed-ratio--3by1
  .flexEmbed-ratio--2by1
  .flexEmbed-ratio--16by9
  .flexEmbed-ratio--4by3
  .flexEmbed-content

.hero
  .hero-content
.hero--slideshow
.hero--graphic

.modal
  .modal-close
  .modal-header
  .modal-content
  .modal-footer

.navbar
  
.pagination
  
```


## States
State classes are prefixed with a keyword that makes sense for the state.

```
.is-active
.is-animating
.is-hidden

```


## Objects
Object classes are prefixed with `o-`

```
.o-nav
.o-nav--fit
.o-nav--stacked

.o-island
.o-island--sm
.o-island--lg

/** 
 * Media 
 *
 * http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/
 */
.o-media
  .o-media-img
  .o-media-img--rev
  .o-media-body

/** 
 * Flag 
 *
 * http://csswizardry.com/2013/05/the-flag-object/
 */
.o-flag
  .o-flag-img
  .o-flag-body 
.o-flag--top
.o-flag--bottom
.o-flag--rev

```


## Utility 
Utility classes are prefixed with `u-`

```
.u-baseSpacing
.u-baseSpacing--top
.u-baseSpacing--bottom
.u-baseSpacing--left
.u-baseSpacing--right

.u-clearfix

.u-pullLeft
.u-pullRight

.u-textBreak
.u-textLeft
.u-textCenter
.u-textRight
.u-textAllcaps
.u-textLowercase
.u-textNoWrap
.u-textTruncate
.u-textLoud
.u-textQuiet

```

---

## Credits

Heavily inspired by these amazing projects & people:
- [CSS Components, Modifiers, and Subcomponents Collection](https://github.com/bjankord/CSS-Components-Modifiers-And-Subcomponents-Collection)
- [SUIT CSS](https://suitcss.github.io/) by [Nicolas Gallagher](https://twitter.com/necolas)
- [Object Oriented CSS](https://github.com/stubbornella/oocss/wiki) by [Nicole Sullivan](https://twitter.com/stubbornella)
- [SMACSS](http://smacss.com) by [Johnathan Snook](https://twitter.com/snookca)
- [BEM Methodology](http://bem.info/) by Yandex
- [Inuit CSS](http://inuitcss.com/) by [Harry Roberts](https://twitter.com/csswizardry)
- [A BEM syntax with UX in mind](http://montagestudio.com/blog/2013/10/24/bem-syntax-with-ux-in-mind/)
- [Bootstrap](http://getbootstrap.com/)

## License
[MIT License](https://github.com/ItsMeAra/CSS-Naming-Conventions/blob/master/LICENSE)
