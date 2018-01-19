### Description
An Article Preview molecule contains a topic label (optional), an article title, a description, and optionally either an image or a Youtube embed and metadata that includes data and read/playtime. Variants are defined based on what fields are needed in each variant, i.e. image or video. The order of elements is determined using flexbox where different from the base pattern.

Variants are managed by use of pseudo-patterns.

- "Article Preview Small Image" is the variant of this pattern that includes a smaller image.
- "Article Preview Video" is the variant of this pattern that includes a video rather than an image.
- "Article Preview Related" is the variant of this pattern that includes an image and title.
- "Article Preview Related No Image" is the variant of this pattern that includes a linked title.

[EWL-4281](https://issues.ama-assn.org/browse/EWL-4281)

~~~
topic_article_preview {
  title_only: string / optional
    type: string / required
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
    }
    image {
      alt:
        type: string / required
      src:
        type: string (url) / required
      height:
        type: string / required
      width:
        type: string / required
    }
    video: string / optional
    related: string / optional
    small: string / optional
    class: string / optional
    paragraph {
      text:
        type: string
    }
    
}
~~~