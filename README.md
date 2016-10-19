# \<xenon-modal\>

Polymer element able to open insde a modal any custom element, very useful if you have to open many modals; using xenon-modal you can do it in a programatic way, avoiding to have several paper-dialog in your html code.

## Usage

First, include the <xenon-modal> tag in yout html


```
<xenon-modal></xenon-modal>
```

Then you can get the component instance

```
const modal = document.querySelector('xenon-modal');
```

## Methods

### showElement(elementName, [properties]);

Instances a given custom element and opens the modal, setting the properties passed as argument.

Example:

```
modal.showElement('my-element', {name: 'Foo', age: 'bar'});
```

### close();

Closes the opened modal.

```
modal.close();
```

### getElement()

Once showElement has been called, this method returns the custom element instance inside xenon-modal

### isOpened()

Return the current state of the modal (true or false).

### getElementProperty(propertyName)

If a custom element is created inside xenon-modal, returns the value of a given property

Example:
```
modal.getElementProperty('name');
```

## Custom properties

* --close-icon-top
* --close-icon-right
* --content-bgcolor
* --content-padding
