# React-Tappable Changelog

## v0.3.3 / 2015-02-19

### Added

- Support for `data-` and `aria-` props on the Component, thanks [Tom Hicks](https://github.com/tomhicks-bsf)

## v0.3.2 / 2015-02-19

### Fixed

- Cleanup around removal of Reactify, build-examples is working again

## v0.3.1 / 2015-02-18

### Fixed

- Reactify is no longer included as a Browserify transform, thanks [Naman Goel](https://github.com/nmn)

## v0.3.0 / 2015-02-07

This release restructured the code so that most methods are now on a Mixin, which is used by the Component (`module.exports`);

You can now mix `react-tappable` into your own Components by using the Mixin directly:

```
var Tappable = require('react-tappable');

var MyComponent = React.createComponent({
	mixins: [Tappable.Mixin],
	/* ... */
});
```
