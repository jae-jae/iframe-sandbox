# iframe-sandbox
动态创建iframe沙箱

## Usage

html
```html
<div id="app" style="height: 500px;width: 800px">
<!--  insert iframe -->
</div>
```

js
```javascript
fetch('http://xxx.com/index.html').then((r)=>{
  return r.text();
}).then((html)=>{
  var a = document.querySelector('#app');
  iframe.create(a,html)
})
```
