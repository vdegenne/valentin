# valentin

valentin is a small "framework" to use with Polymer 2.0.
It provides some useful functions and custom elements, which used together can help to quickly develop web-apps.

## Installation

install `valentin` using bower

```
bower install valentin --save
```

and just import `valentin.html` in your project

```html
<link rel="import" href="/bower_components/valentin/valentin.html">
```


## app-toaster

you can use the `app-toaster` and `Valentin.toast()` to quickly embed a toaster in your app.

```html
<template>
  <app-toaster>
    ...
    <button on-click="toast_something">toast something</button>
    ...
  </app-toaster>
</template>
<script>
class MyElement extends Polymer.Element
{
  ...
  
  toast_something () {
    /**
     * `0` means normal
     * use `1` to color the toaster in red in case of an error
     */
    Valentin.toast(this, 'just saying hi', 0);
  }
  
  ...
}
</script>
```

