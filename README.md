# ObjectPosition plugin for [PhotoSwipe](https://github.com/dimsemenov/PhotoSwipe)

ObjectPosition — is a [PhotoSwipe](https://github.com/dimsemenov/PhotoSwipe)
plugin that improves `object-position` property handling when cropped thumbnails
are used.

## Improvements

 1. Fixes thumbnail jumping animation while opening/closing lightbox.
 2. Make sure that the initially zoomed image will show the same region of the image
    as we saw in cropped thumbnail.

## Usage

```js
import PhotoSwipeLightbox from '/assets/photoswipe/dist/photoswipe-lightbox.esm.js';
import ObjectPosition from '/assets/photoswipe-object-position.js';

const lightbox = new PhotoSwipeLightbox({
  gallery: '#my-gallery',
  children: 'a',
  pswpModule: () => import('/assets/photoswipe/dist/photoswipe.esm.js')
});

new ObjectPosition(lightbox);

lightbox.init();
```
