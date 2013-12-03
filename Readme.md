# Bootstrap Pagy

## About

Bootstrap Pagy is a jQuery plugin that simplifies the use of the Bootstrap Pagination component.

## Why

There are already other pagination plugins using the Bootstrap markup: [boogpag](http://botmonster.com/jquery-bootpag) and [Bootstrap Paginator](http://bootstrappaginator.org/).

In contrast to those plugins Bootstrap Pagy provides a fixed inner window (compare the demos to see what this means). The page layout algorithm used is inspired by [Kaminari](https://github.com/amatsuda/kaminari).

## Features

* Custom previous and next button
* Custom first and last button
* Custom inner window size (default 2)
* Custom outer window size (default 0)
* Set current page and total pages programmatically
* Code under Apache License
* Only depends on jQuery (for Javascript) and Bootstrap (for Markup)

## Demo

http://medihack.github.io/bootstrap-pagy/demo/

## Download

* [Development (not minified)](https://raw.github.com/medihack/bootstrap-pagy/master/src/bootstrap-pagy.js)
* [Production (minified)](https://raw.github.com/medihack/bootstrap-pagy/master/src/bootstrap-pagy.min.js)

## Usage

Minimal usage:
```js
$(".pagination").pagy({
  totalPages: 20,
  currentPage: 3,
  page: function(page) {
    // do something when page changed;
    return true;
  }
});
```

All available (default) options:
```js
$(".pagination").pagy({
    currentPage: null,
    totalPages: null,
    innerWindow: 2,
    outerWindow: 0,
    first: '&laquo;',
    prev: '&lsaquo;',
    next: '&rsaquo;',
    last: '&raquo;',
    gap: '..',
    truncate: false,
    page: function(page) { return true }
});
```

Set current page programmatically:
```js
$(".pagination").pagy("page", 4);
```

Set current page and total pages programmatically:
```js
$(".pagination").pagy("page", 4, 20);
```

## License

Licensed under the Apace License:
http://opensource.org/licenses/Apache-2.0

Copyright(c) 2013 Kai Schlamp
