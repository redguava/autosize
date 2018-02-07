## Red Guava fork
I forked this to get rid of the problem with iOS jumping the scroll position to under the keyboard. There is a [similar PR](https://github.com/jackmoore/autosize/pull/352) in the autosize repo but the owner feels it is a regression on desktop since it doesn't handle scrolling parents with nested overflow. I don't believe we have any cases where that would cause a problem for us.

## Summary

Autosize is a small, stand-alone script to automatically adjust textarea height to fit text.

#### Demo

Full documentation and a demo can be found at [jacklmoore.com/autosize](http://jacklmoore.com/autosize)

#### Install via NPM
```bash
npm install autosize
```

#### Browser compatibility

Chrome | Firefox | IE | Safari | iOS Safari | Android | Opera Mini | Windows Phone IE
------ | --------|----|--------|------------|---------|------------|------------------
yes    | yes     | 9  | yes    | yes        | 4       | ?          | 8.1

#### Usage

The autosize function accepts a single textarea element, or an array or array-like object (such as a NodeList or jQuery collection) of textarea elements.

```javascript
// from a NodeList
autosize(document.querySelectorAll('textarea'));

// from a single Node
autosize(document.querySelector('textarea'));

// from a jQuery collection
autosize($('textarea'));
```

Released under the [MIT License](http://www.opensource.org/licenses/mit-license.php)
