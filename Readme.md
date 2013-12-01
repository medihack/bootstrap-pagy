# Bootstrap Pagy

## About

Bootstrap Pagy is a jQuery plugin that simplifies the use of the Bootstrap Pagination component.

## Features

* Custom previous and next button
* Custom first and last button
* Custom inner window size (default 2)
* Custom outer window size (default 0)
* Set current page and total pages programmatically
* Code under Apache License
* Only depends on jQuery (for Javascript) and Bootstrap (for Markup)

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
    left: 0,
    right: 0,
    first: '&laquo;',
    prev: '&lsaquo;',
    next: '&rsaquo;',
    last: '&raquo;',
    gap: '...',
    truncate: true,
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

## Demo

http://medihack.github.io/bootstrap-pagy/demo/

## License

Licensed under the Apace License:
http://opensource.org/licenses/Apache-2.0

Copyright(c) 2013 Kai Schlamp
