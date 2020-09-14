# Bootstrap Responsive Grid
A package that allows you to define different gutters and container margins for each breakpoint.

This package can be used as a wrapper around [Bootstrap 4](https://github.com/twbs/bootstrap) and provides variables to customise the gutter widths and the container margins separately for each break-points and independently of each other.

## Usage

### Installation
Install using npm, e.g.: 

`npm install --save-dev https://github.com/BenceSzalai/bootstrap-responsive-grid.git`

### Setup
You can use `scss/bootstrap.scss` or `scss/bootstrap-grid.scss` of this package the same way as you would use the same files provided by Bootstrap.

In your main scss file instead of `@import "~bootstrap";` you can use `@import "~bootstrap-responsive-grid";`.

If you are using only the Bootstrap grid, instead of `@import "~bootstrap/scss/bootstrap-grid";` you can use `@import "~bootstrap-responsive-grid/scss/bootstrap-grid";`.

If you would like more granular control over the specific Bootstrap components, you can make a copy of `scss/bootstrap/bootstrap.scss`, edit each `@import` that does not start with `"~bootstrap/...` to start with `"~bootstrap-responsive-grid/scss/bootstrap/...` and remove any lines corresponding to components you don't need. E.g.:
```[SCSS]
@import "~bootstrap/scss/functions";
@import "~bootstrap/scss/variables";
@import "~bootstrap-responsive-grid/scss/variables";
@import "~bootstrap/scss/mixins";
@import "~bootstrap-responsive-grid/scss/bootstrap/mixins/grid-framework";
@import "~bootstrap-responsive-grid/scss/bootstrap/mixins/grid";
@import "~bootstrap-responsive-grid/scss/mixins";
@import "~bootstrap/scss/root";
@import "~bootstrap/scss/reboot";
@import "~bootstrap/scss/type";
@import "~bootstrap/scss/images";
@import "~bootstrap/scss/code";
@import "~bootstrap-responsive-grid/scss/bootstrap/grid";
@import "~bootstrap/scss/tables";
@import "~bootstrap/scss/forms";
@import "~bootstrap/scss/buttons";
```

### Configuration

Similar to Bootstrap, the package uses SCSS variables as the entry point for your settings. The default configuration matches the out of the box default behaviour of Bootstrap: 30px for gutters and 15px for container margins on all resolutions.

To customise these, add the following SCSS map variables before importing the package files:
```[SCSS]
$grid-gutter-widths: (
  xs: 10px,
  sm: 20px,
  md: 30px,
  lg: 40px,
  xl: 60px
);

$grid-container-margins: (
  xs: 20px,
  sm: 30px,
  md: 40px,
  lg: 60px,
  xl: 80px
);
```

The `xs` part is mandatory in both maps. The other breakpoints from `sm` and above are optional. Any breakpoint not provided in the map will use the same value from the breakpoint below.

To take full control of the Bootstrap grid system you may also want to customise the `$container-max-widths` and `$grid-breakpoints` default Bootstrap map variables. For details see `scss/_variables.scss` in Bootstrap.

## Other

This is not a well tested solution. It works fine for me, but your mileage may vary. If you find any issues, please report [here](https://github.com/BenceSzalai/bootstrap-responsive-grid/issues), and I'll try to fix it so this package can be improved. Pull requests are welcome as well.
