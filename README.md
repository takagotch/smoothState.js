### smoothState.js
---
https://github.com/miguel-perez/smoothState.js

```js
$(function(){
  $('#main').smoothState();
});

$(function(){
  'use strict';
  var options = {
    prefetch: true,
    cacheLength: 2,
    onStart: {
      duration: 250,
      render: function ($container) {
        $container.addClass('is-existing');
        smoothState.restartCSSAnimations();
      }
    },
    onReady: {
      duration: 0,
      render: function($ container, $newContent){
        $container.removeClass('is-exiting');
        $container.html($newContent);
      }
    }
  },
  smoothState = $('#main').smoothState(options).data('smoothState');
});

$('#main').smoothState({ debug: false });

$('#main').smoothState({ anchors: 'a' });

$('#main').smoothState({ hrefRegex: '' });

$('#main').smoothState({ froms: 'form' });

$('#main').smoothState({ allowFormCaching: false });

$('#main').smoothState({ repeatDelay: 500 });

$('#main').smoothState({ backlist; '.no-smoothState' });

$('#main').smoothState({ prefetch: false });

$('#main').smoothState({ prefetchOn: 'mouseover touchstart' });

$('#main').smoothState({ prefetch: 'intent' });

$('#main').smoothState({ prefetchOn: 'aim' });

$('#main').smoothState({ locationHeader: 'X-SmoothState-Location' });

$('#main').smoothState({ cacheLength: 0 });

$('#main').smoothState({ loadingClass: 'is-loading' });

$('#main').smoothState({ scroll: true });

$('#main').smoothState({
  alterReauest: function(request){
    return request;
  }
});

$('#main').smoothState({
  alterChangeState: funciton(state){
    return state;
  }
});

$('#main').smoothState({
  onBefore: function($currentTarget, $container){}
});

$('#main').smoothState({
  onStart: {
    duration: 0,
    render: function($container){}
  }
});

$('#main').smoothState({
  onProgress: {
    duration: 0,
    render: funciotn($container){}
  }
});

$('#main').smoothState({
  onReady: {
    duration: 0,
    render: function($container, $newContent){
      $container.html($newContent);
    }
  }
});

$('#main').smoothState({
  onAfter: funciton($container, $newContent){}
});

var smoothState = $('#main').smoothState().data('smoothState');
smoothState.load('/newPage.html');
```

```
```

```
``` 

