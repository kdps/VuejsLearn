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

v-bind:class="{className: bool[binding data] }"

v-bind:class="{classObject}"

```
data: {
  classObject: {
    active: true,
    'text-danger': false
  }
}
```

v-if="{bool}" : Check that bool is true

v-for="{var} in {array}" : do loop in array

v-on:{eventType}="{method}" : do event when bind event

v-model="{Globally binding data}" : Update data when bind is updated

### Constructor Parameter

el : Element Selector (... #id, .class)

watch : Set Watch Instance (Watch is call method when data is changed)

data : Element Data

 -> message : Globally binding data

computed : Define multiple functions in this properties, and it has getter and setter method

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

props : ["{Properties}"] : Set Properties In Data Of Binding Object

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

# Instance

### Usage

```
{Vue Object}.$watch("domain", function(){
});
```

