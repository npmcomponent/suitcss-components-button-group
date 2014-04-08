*This repository is a mirror of the [component](http://component.io) module [suitcss/components-button-group](http://github.com/suitcss/components-button-group). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/suitcss-components-button-group`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# SUIT ButtonGroup

CSS for visually grouping buttons.

Read more about [SUIT's design principles](https://github.com/suitcss/suit/).

## Installation

* [Component(1)](https://github.com/component/component): `component install suitcss/components-button-group`
* [npm](http://npmjs.org/): `npm install suitcss-components-button-group`
* [Bower](http://bower.io/): `bower install suit-components-button-group`

## Available classes

* `ButtonGroup` - The core component.
* `ButtonGroup--hz` - Horizontally arranged buttons.
* `ButtonGroup-item` - A `ButtonGroup` sub-object used to contain buttons.

The plugin file provides the following classes:

* `ButtonGroup--borderCollapse` - Collapse the borders between buttons.

## Configurable variables

* `var-font-size-ButtonGroup` - The font-size to use. Defaults to `1rem`.

## Use

An element with the `ButtonGroup` class must be used to wrap a collection of
elements with the `ButtonGroup-item` class. The `ButtonGroup` component *must*
only contain `ButtonGroup-item` components as children.

The button group items must contain
[Button](https://github.com/suitcss/components-button) components.

```html
<div class="ButtonGroup">
  <div class="ButtonGroup-item">
    <a class="Button" href="{{url}}">Dashboard</a>
  </div>
  <div class="ButtonGroup-item">
    <a class="Button" href="{{url}}">Settings</a>
  </div>
  <div class="ButtonGroup-item">
    <a class="Button" href="{{url}}">
      Account
      <span class="Icon Icon--cog"></span>
    </a>
  </div>
</div>
```

## Testing

Install [Node](http://nodejs.org) (comes with npm).

```
npm install
```

To generate a build:

```
npm run build
```

To generate the testing build.

```
npm run build-test
```

Basic visual tests are in `test.html`.

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 9+
