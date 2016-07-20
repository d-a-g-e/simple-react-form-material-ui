# Materia UI - Simple React Form

[Simple React Form](https://github.com/nicolaslopezj/simple-react-form) is a powerful framework that simplifies the use of forms in React. This is a set of components that use Material UI.

To use this fields, import this package once at startup

```js
import 'simple-react-form-material-ui'
```

## Components

List of the components

### [Checkbox](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/checkbox.jsx)

Name: ```checkbox```

Type: ```Boolean```

### [Date Picker](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/date-picker.jsx)

Renders the [material-ui date picker](http://www.material-ui.com/#/components/date-picker)

Name: ```date-picker```

Type: ```Date```

### [Multiple Checkbox](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/multiple-checkbox.jsx)

Select multiple items from a array

Name: ```multiple-checkbox```

Type: ```[String|Number]```

Props:
- ```options```: A array of
  - ```label``` ```String```: The label of the option
  - ```value``` ```String|Number```: The value
  - ```description``` ```String``` Optional: A description that will be rendered below the option

### [Radio](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/radio.jsx)

Select one item from a array

Name: ```radio```

Type: ```String|Number```

Props:
- ```options```: A array of
  - ```label``` ```String```: The label of the option
  - ```value``` ```String|Number```: The value
  - ```description``` ```String``` Optional: A description that will be rendered below the option

### [Select With Method](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/select-with-method.jsx)

A text field that searchs items with meteor methods

Name: ```select-with-method```

Type: ```String|Number```

Props:
- ```multi``` ```Boolean``` Optional: Allow to select multiple items.
- ```methodName``` ```String```: Meteor method that recieves the search string and returns an array of
  - ```label``` ```String```: The visible text.
  - ```value``` ```String|Number```: The value.
  - ```color``` ```String``` Optional: The background color of the chip
  - ```image``` ```String``` Optional: The url of the image
  - ```initals``` ```String``` Optional: The initals of the chip. Don't provide this if image is present.
- ```labelMethodName``` ```String```: Meteor method that recieves the value and must return the item description. If ```multi``` is set to true, this will recieve an array of the values and must return an array with the items descriptions in the same order. Item description is the same as the one returned in ```methodName```:
  - ```label``` ```String```: The visible text.
  - ```value``` ```String|Number```: The value.
  - ```color``` ```String``` Optional: The background color of the chip
  - ```image``` ```String``` Optional: The url of the image
  - ```initals``` ```String``` Optional: The initals of the chip. Don't provide this if image is present.
- ```connection``` Optional, defaults to ```Meteor```: A Meteor connection.
- ```waitTime``` Optional, defaults to ```400```: Time with no changes that activates the search.
- ```create``` ```Function``` Optional: A function that creates a document and pass the value in a callback.
- ```createLabel``` ```Function``` Optional: A function that recieves the search input and returns the create label.
- ```canCreate``` ```Function``` Optional, defaults to ```() => true```: A function that recieves the search input and returns a ```Boolean``` indicating if ```create``` can be called.

### [Select](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/select.jsx)

Select one item from a array in a select field

Name: ```select```

Type: ```String|Number```

Props:
- ```options```: A array of
  - ```label``` ```String```: The label of the option
  - ```value``` ```String|Number```: The value

### [Tags](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/tags.jsx)

Create a array of Strings.

Name: ```tags```

Type: ```[String]```

### [Text](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/text-field.jsx)

Name: ```text```

Type: ```String```

Props:
- ```fieldType``` ```String``` Optional: The type of the input. Example: number, email, password.

### [Textarea](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/textarea.jsx)

A String with multiple lunes

Name: ```textarea```

Type: ```String```

### [Toggle](https://github.com/nicolaslopezj/simple-react-form-material-ui/blob/master/src/fields/toggle.jsx)

Name: ```toggle```

Type: ```Boolean```
