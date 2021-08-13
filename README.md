# Bootstrap Offcanvas

Hidden sidebar, perfect for use in the form of additional navigation, for example in ecommerce projects or dashboards.

## How it works

Offcanvas is a sidebar component that can be toggled via JavaScript to appear from the left, right, or bottom edge of the viewport. Buttons or anchors are used as triggers that are attached to specific elements you toggle, and `data` attributes are used to invoke our JavaScript.

* Offcanvas shares some of the same JavaScript code as modals. Conceptually, they are quite similar, but they are separate plugins.
* Similarly, some [source Sass](https://mdbootstrap.com/docs/standard/extended/offcanvas/#section-sass) variables for offcanvas’s styles and dimensions are inherited from the modal’s variables.
* When shown, offcanvas includes a default backdrop that can be clicked to hide the offcanvas.
* Similar to modals, only one offcanvas can be shown at a time.

**Heads up!** Given how CSS handles animations, you cannot use `margin` or `translate` on an `.offcanvas` element. Instead, use the class as an independent wrapping element.

## Examples

#### Offcanvas components

Below is an offcanvas example that is shown by default (via `.show` on `.offcanvas`). Offcanvas includes support for a header with a close button and an optional body class for some initial `padding`. We suggest that you include offcanvas headers with dismiss actions whenever possible, or provide an explicit dismiss action.

```html
<div class="offcanvas offcanvas-start show" tabindex="-1" id="offcanvas" aria-labelledby="offcanvasLabel"
  data-mdb-backdrop="false" data-mdb-scroll="true">
  <div class="offcanvas-header">
    <h5 class="offcanvas-title" id="offcanvasLabel">Offcanvas</h5>
    <button type="button" class="btn-close text-reset" data-mdb-dismiss="offcanvas" aria-label="Close"></button>
  </div>
  <div class="offcanvas-body">
    Content for the offcanvas goes here. You can place just about any Bootstrap component or custom elements here.
  </div>
</div>
```

#### Much more examples and a detailed description can be found at [📄 Offcanvas documentation page](https://mdbootstrap.com/docs/standard/extended/offcanvas/)
