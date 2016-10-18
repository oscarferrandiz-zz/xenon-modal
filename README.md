# \<xenon-modal\>

Modal Polymer element able to open insde a modal any custom element.

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

### getElement()

Once showElement has been called, this method returns the custom element instance inside xenon-modal

### isOpened()

Return the current state of the modal (true or false).

### getElementProperty

If a custom element is created inside xenon-modal, returns the value of a given property

Example:
```
modal.getElementProperty('name');
```
