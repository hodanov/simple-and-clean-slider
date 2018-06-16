# A responsive jQuery slider

This is the very simple and clean responsive jQuery slider.

The image size is adjusted automatically, so there is no need to resize image files.

## LICENSE

All source code is available jointly under the MIT License and the Beerware License. Please see
[LICENSE.md](LICENSE.md) for details.

## Demo

To see the slider, clone the repo.

## Requirements

The slider requires the following to run:

- jQuery

## Usage

### Set css and js files

Please set [style.css](https://gitlab.com/hodanov/simple-and-clean-slider/tree/master/css/style.css) and [script.js](https://gitlab.com/hodanov/simple-and-clean-slider/tree/master/js/script.js) in the appropriate place, and import them.

### Structure

The slider with the following HTML structure:

- `slide-window` the main container
  - `slide-wrapper` contains __slides__ and decide width
    - `slide` each __slide item__ of the slider
      - `a` a link
        - `slide-image` the div element, which can include __slide image__
        - `slide-caption` the div element, which can include some __text__

### 1. slide-window

The `slide-window` is the main container. It can contain slide items.

```
<div class="slide-window">
  <div class="slide-wrapper" style="width: 300%;">
    <!-- slide items -->
  </div>
</div>
```

### 2. slide-wrapper

The `slide-wrapper` is the 2nd main container. It can decide width:

- _width = x * 100(%)_
  - _x_ is a number of slide items

If there are two slide items, add `style="width: 200%;"` in `slide-wrapper`.

```
<div class="slide-window">
  <div class="slide-wrapper" style="width: 200%;">
    <div class="slide">
      <!-- slide item 1 -->
    </div>
    <div class="slide">
      <!-- slide item 2 -->
    </div>
  </div>
</div>
```

### 3. slide item

The `slide` is the slide item, which can include `slide-image` and `slide-caption`.

```
<div class="slide">
  <a href="#" target="_blank">
    <div class="slide-image" style="background-image: url(img/slide1.jpg)">
    </div>
    <div class="slide-caption">
      <h2>AUTONOMY</h2>
      <p>Always keep the sun in your heart.</p>
    </div>
  </a>
</div>
```

Add `style="background-image: url(IMAGE_FILE)"` to `slide-image`. The image size is adjusted automatically.

## Author

[Hodaka Sakamoto](https://hodalog.com/)
