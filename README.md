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
.list--group

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
.table--responsive

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

.badge
.badge--sm
.badge--lg

.btnGroup

.carousel
  .carousel-item
  .carousel-controls
  
.dropdown
  .dropdown-trigger
  .dropdown-content

.grid
.grid--centered
.grid--collapsed
  .grid-row
  .grid-col
  .grid-col--1
  .grid-col--2
  .grid-col--3
  .grid-col--4
  .grid-col--5
  .grid-col--6
  .grid-col--7
  .grid-col--8
  .grid-col--9
  .grid-col--10
  .grid-col--11
  .grid-col--12
  .grid-col--xsm1
  .grid-col--xsm2
  .grid-col--xsm3
  .grid-col--xsm4
  .grid-col--xsm5
  .grid-col--xsm6
  .grid-col--xsm7
  .grid-col--xsm8
  .grid-col--xsm9
  .grid-col--xsm10
  .grid-col--xsm11
  .grid-col--xsm12   
  .grid-col--sm1
  .grid-col--sm2
  .grid-col--sm3
  .grid-col--sm4
  .grid-col--sm5
  .grid-col--sm6
  .grid-col--sm7
  .grid-col--sm8
  .grid-col--sm9
  .grid-col--sm10
  .grid-col--sm11
  .grid-col--sm12  
  .grid-col--md1
  .grid-col--md2
  .grid-col--md3
  .grid-col--md4
  .grid-col--md5
  .grid-col--md6
  .grid-col--md7
  .grid-col--md8
  .grid-col--md9
  .grid-col--md10
  .grid-col--md11
  .grid-col--md12  
  .grid-col--lg1
  .grid-col--lg2
  .grid-col--lg3
  .grid-col--lg4
  .grid-col--lg5
  .grid-col--lg6
  .grid-col--lg7
  .grid-col--lg8
  .grid-col--lg9
  .grid-col--lg10
  .grid-col--lg11
  .grid-col--lg12  
  .grid-col--xlg1
  .grid-col--xlg2
  .grid-col--xlg3
  .grid-col--xlg4
  .grid-col--xlg5
  .grid-col--xlg6
  .grid-col--xlg7
  .grid-col--xlg8
  .grid-col--xlg9
  .grid-col--xlg10
  .grid-col--xlg11
  .grid-col--xlg12      

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

.icon
.icon--xsm
.icon--sm
.icon--lg
.icon--xlg

.siteWrapper  
.siteHeader
.siteFooter

.strip
.strip--light
.strip--dark
.strip--xsm
.strip--sm
.strip--lg
.strip--xlg
  
```


## States
State classes are prefixed with a keyword that makes sense for the state.

```
.is-active
.is-animating
.is-collapsed
.is-hidden
.is-pressed
.is-selected

```


## Objects
Object classes are prefixed with `o-`

```
.o-flexEmbed
  .o-flexEmbed-ratio
  .o-flexEmbed-ratio--3by1
  .o-flexEmbed-ratio--2by1
  .o-flexEmbed-ratio--16by9
  .o-flexEmbed-ratio--4by3
  .o-flexEmbed-content

.o-nav
.o-nav--fit
.o-nav--stacked
.o-nav--pagination
.o-nav--keywords

.o-island
.o-island--xsm
.o-island--sm
.o-island--lg
.o-island--xlg

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

u-block
u-hidden
u-hiddenVisually 
u-inline
u-inlineBlock 
u-table 
u-tableCell 
u-tableRow 

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
