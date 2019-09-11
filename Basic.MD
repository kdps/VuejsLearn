# Attributes And Constructor Variables

### Usage

```
var App = new Vue({
  el: "",
  ...
});
```

### Element Properties

v-bind:{attributes}="{Globally binding data}" : Bind to element

v-if="{bool}" : Check that bool is true

v-for="{var} in {array}" : do loop in array

v-on:{eventType}="{method}" : do event when bind event

v-model="{Globally binding data}" : Update data when bind is updated

### Constructor Parameter

el : Element Selector (... #id, .class)

data : Element Data

 -> message : Globally binding data

methods : Define functions

```
methods: {

    reverseMessage: function () {
    
      this.message = this.message.split('').reverse().join('')
      
    }
    
}
```

# Component

### Usage

```
Vue.component('domain', {
  template: '{HTML Template}'
})
```

### Constructor Variables

template: "{Template Code}" : Set HTML Template

props : ["{Properties}"] : Set Properties

```
Vue.component('todo-item', {
  props: ['todo'],
  template: '<li>{{ todo.text }}</li>'
})

var app7 = new Vue({
  el: '#app-7',
  data: {
    groceryList: [
      { id: 0, text: 'Vegetables' },
      { id: 1, text: 'Cheese' },
      { id: 2, text: 'Whatever else humans are supposed to eat' }
    ]
  }
})
```
