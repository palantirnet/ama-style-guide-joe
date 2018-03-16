---
el: '.ama__info-card'
title: 'Information Card'
---

### Description
Information card molecules contain a heading that denotes the card type (required), an image (optional), and format-able text (required). Variants are defined based on what fields are included and type of information (or card type).

Variants are managed by use of pseudo-patterns.

- ["Info Card as Media Contact"](?p=molecules-info-card-as-media-contact) is the variant of this pattern that includes a smaller image and appears on within the [Partner Information](#) on a [Press Release Page]?p=pages-press-release).

[EWL-4487](https://issues.ama-assn.org/browse/EWL-4487)

### Variables
~~~
{
  infoCard: {
    heading {
      level:
        type: string / required
      text:
        type: string / required
      class:
        type: string / optional
    },
    image {
      alt:
        type: string / required
      src:
        type: string (url) / required
      height:
        type: string / required
      width:
        type: string / required
    },
    paragraph {
      text:
        type: string
      class:
        type: string / optional
    },
    link {
      href:
        type: string / required
      text:
        type: string / required
      class:
        type: string / optional
      target:
        type: string / optional
      title:
        type: string / optional
      icon:
        type: string / optional
    }
  }
}
~~~