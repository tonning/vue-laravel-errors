### Installation
Pull in by running: `yarn add @tonning/vue-laravel-old`

In your app.blade.php layouts file add:
```html
<script type="text/javascript">
    let Laravel = {
        error: {!! json_encode($errors->messages()) !!},
    };
</script>
```

In your app.js file
* `import Vue from 'vue'`  
* `import VueLaravelOld from 'vue-laravel-error'` 
* `Vue.use('vue-laravel-error', Laravel.error)`  


### Usage
Now you can use it in Vue and your Vue components  
`Vue.$error.get('email')` or `this.$error.get('email')`
