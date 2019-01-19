### jquery.hotkeys
---
https://github.com/RobertWHurst/KeyboardJS

```js
keyboardJS.bind('a', function(e){
  console.log('a is pressed');
});
keyboardJS.bind('a + b', function(e){
  console.log('a and is pressed');
});
keyboardJS.bind('a + b > c', function(e){
  console.log('a and b then c is pressed');
});
keyboardJS.bind(['a + b > c', 'z + y > z'], function(e){
  console.log('a and b then c or z and then z is pressed');
});
keyboardJS.bind('', function(e){
  console.log('any key was pressed');
});

keyboardJS.bind('a', function(e){
  console.log('a is pressed');
}, function(e){
  console.log('a is released');
});
keyboradJS.bind('a', null, function(e){
  console.log('a is released');
});

keyboardJS.bind('a', function(e){
  e.preventRepeat();
  console.log('a is pressed');
});

keyboardJS.unbind('a', previouslyBoundHandler);

keyboardJS.bind('a', function(e){});
keyboardJS.bind('b', function(e){});
keyboardJS.bind('c', function(e){});
keyboardJS.setContext('index');
keyboardJS.bind('1', function(e){});
keyboardJS.bind('2', function(e){});
keyboardJS.bind('3', function(e){});

keyboardJS.bind('foo');
keyboardJS.bind('x', function(e){});
keyboardJS.bind('y', function(e){});
keyboardJS.bind('z', function(e){});

myRouter.on('GET /', function(e){
  keyboardJS.setContext('index');
});
myRouter.on('GET /foo', function(e){
  keyboardJS.setContext('foo');
});
var contextName = keyboardJS.getContext();
keyboardJS.withContext('bar', function(){
  keyboardJS.bind('7', function(e){});
  keyboardJS.bind('8', function(e){});
  keyboardJS.bind('9', function(e){});
});

keyboardJS.pause();
keyboardJS.resume();
keyboardJS.reset();

keyboardJS.pressKey('a');
keyboardJS.pressKey(65);
keyboardJS.releaseKey('a');
keyboardJS.releaseKey(65);
keyboardJS.releaseAllKeys();

keyboardJS.watch();
keyboardJS.watch(myWin, myDoc);
keyboardJS.watch(myForm);
keyboardJS.watch(myWin, myForm);
keyboardJS.stop();
```


```
```

```
```

