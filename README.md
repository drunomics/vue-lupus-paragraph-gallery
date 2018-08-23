# vue-lupus-paragraph-gallery
Vue gallery paragraph component.



## Install

via npm:
`npm install https://github.com/drunomics/vue-lupus-paragraph-gallery.git`


import it:

```
import { PgGallery } from 'vue-lupus-paragraph-gallery';

Vue.component('pg-gallery', PgGallery);
```

## Properties
You can pass the following props:

- `data-name` ( string )
  The gallery's name.
- `data-images` ( string )
  JSON representation of the image array.
    - [{'src': '/path/to/image', 'alt': 'The alt text'}]

## Example
```
<pg-gallery
  data-name="Quote"
  data-images="[{'src': '/path/to/image', 'alt': 'The alt text'}]"
>
```