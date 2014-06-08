
# Clipboard

  Clipboard library.

## Installation

```
$ component install component/clipboard
```

## Example

```js
var Clipboard = require('clipboard');
var clip = new Clipboard(window);

clip.on('paste', function(e){
  e.items.forEach(function(item){
    console.log(item);
  });
});

clip.on('cut', function(){
  console.log('cut');
});

clip.on('copy', function(e){
  console.log('copy');
});
```

## API

### Clipboard#bind()

  Bind event handlers. This is done for you in the constructor.

### Clipboard#unbind()

  Unbind event handlers.

## Links

  - w3c [clipboard apis](http://www.w3.org/TR/clipboard-apis/)
  - [Can I Use...?](http://caniuse.com/#search=clipboard)
  - Mozilla [MDN](https://developer.mozilla.org/en-US/docs/Web/API/ClipboardEvent)
  - Microsoft [MSDN](http://msdn.microsoft.com/en-us/library/ie/ms535220%28v=vs.85%29.aspx)


## License

 MIT
