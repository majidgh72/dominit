# dominit
Simple Object to DOM Element generator for JavaScript

Write a Javascript object, convert it to DOM element simply using Dominit!

Ultra lightweight(~0.5kb!) and high performance

Written in VanillaJS



## Simple usage example:

```html

<div id="app"></div>


<script src="/path/to/dominit.min.js"></script>
<script>
var appDOM = {
  el: 'div',
  attrs: {
    class: 'post-body'
  },
  children: [
    {
      el: 'h1',
      text: 'Post title'
    }
  ]
};
  
const App = document.getElementById("app");
const dominit = new Dominit(
  App,
  appDOM
);
dominit.render();
</script>
```

Result of above code will be:
```html

<div id="app">
  <div class="post-body">
    <h1>Post title</h1>
  </div>
</div>
```




