# Element Properties

v-bind:{attributes}="{Globally binding data}" : Bind to element

v-if="{bool}" : Check that bool is true

v-for="{var} in {array}" : do loop in array

v-on:{eventType}="{method}" : do event when bind event

# Constructor Parameter

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
