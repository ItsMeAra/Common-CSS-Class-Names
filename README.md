# Common CSS Class Names

A collection of common CSS name ideas for a naming convention based on [Object Oriented CSS](https://github.com/stubbornella/oocss/wiki) and the [BEM Methodology](http://bem.info/). 

While using these approaches in [my projects](https://css-tricks.com/design-systems-building-future/), I discovered that naming things is easily one of the most frustrating parts of development. In an effort to make it easier on myself and others who feel the same, I've put together a list of commonly used CSS names for elements, components, and utility classes.  

---

## The Naming Convention

My prefered naming convention follows the SUIT CSS [Naming Conventions](https://github.com/suitcss/suit/blob/master/doc/naming-conventions.md) very closely:

```
/* Components (blocks) */
.myComponent {}                     /* Block - camelCase the component (block) name */
.myComponent-descendant {}          /* Element - One dash for a descendant of the component */
.myComponent--modifier {}           /* Modifier - Two dashes for the modifier of the component */

/* Utils */
.u-myHelper {}                      /* Utility classes are prefixed with `u-` */

/* States */
.myComponent.is-active {}           /* State classes are chained */

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
.list--ordered
.list--unOrdered

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
.img--circle
.img--rounded
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

.button
.button--default
.button--primary
.button--secondary
.button--pill
.button--soft
.button--hard
.button--circle
.button--xs
.button--sm
.button--lg
.button--xl
.button--xxl

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
  .accordion-trigger
  .accordion-content
.accordion--vertical
.accordion--horizontal

.badge
.badge--xs
.badge--sm
.badge--lg
.badge--xl

.btnGroup
.btnGroup--stacked

.carousel
  .carousel-item
  .carousel-controls
  
.dropdown
  .dropdown-trigger
  .dropdown-content
  .dropdown-data

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
.navbar--primary
.navbar--secondary

.icon
.icon--xs
.icon--sm
.icon--lg
.icon--xl
.icon--xxl

.siteWrapper  
.siteHeader
.siteFooter

.strip
.strip--light
.strip--dark
.strip--xs
.strip--sm
.strip--lg
.strip--xl

.flexEmbed
  .flexEmbed-ratio
  .flexEmbed-ratio--3x1
  .flexEmbed-ratio--2x1
  .flexEmbed-ratio--16x9
  .flexEmbed-ratio--4x3
  .flexEmbed-content

.nav
.nav--fit
.nav--stacked
.nav--pagination
.nav--keywords

.island
.island--xs
.island--sm
.island--lg
.island--xl

/** 
 * Media 
 *
 * http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/
 */
.media
  .media-img
  .media-img--rev
  .media-body

/** 
 * Flag 
 *
 * http://csswizardry.com/2013/05/the-flag-object/
 */
.flag
  .flag-img
  .flag-body 
.flag--top
.flag--bottom
.flag--rev

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
.is-finished

```


## Utility 
Utility classes are prefixed with `u-`
```
.u-baseMargin
.u-baseMargin--top
.u-baseMargin--bottom
.u-baseMargin--left
.u-baseMargin--right

.u-basePadding
.u-basePadding--top
.u-basePadding--bottom
.u-basePadding--left
.u-basePadding--right

.u-clear
.u-clearfix
.u-clearLeft
.u-clearRight

u-displayBlock
u-displayNone
u-displayHidden 
u-displayInline
u-displayInlineBlock 
u-displayTable 
u-displayTableCell 
u-displayTableRow 

.u-pullLeft
.u-pullRight

.u-textBreak
.u-textLeft
.u-textCenter
.u-textRight
.u-textAllcaps
.u-textLowercase
.u-textUppercase
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
- [BEM Methodology](http://bem.info/) by Yandex
- [Inuit CSS](http://inuitcss.com/) by [Harry Roberts](https://twitter.com/csswizardry)
- [Bootstrap](http://getbootstrap.com/)

## License
[MIT License](https://github.com/ItsMeAra/CSS-Naming-Conventions/blob/master/LICENSE)
