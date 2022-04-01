# ObjectPosition plugin for [PhotoSwipe](https://github.com/dimsemenov/PhotoSwipe)

ObjectPosition — is a [PhotoSwipe](https://github.com/dimsemenov/PhotoSwipe)
plugin that improves `object-position` property handling when cropped thumbnails
are used.

## Improvements

 1. Fixes thumbnail jumping animation while opening/closing lightbox.
 2. Make sure that the initially zoomed image will show the same region of the image
    as we saw in cropped thumbnail.

[View Demo](https://vovayatsyuk.github.io/photoswipe-object-position/)

## Usage

Download the `photoswipe-object-position.js` file and put it to your assets folder.

> Alternatively, you may install the plugin via NPM:
>
> ```
> npm i @vovayatsyuk/photoswipe-object-position
> ```

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
