# FvModal.js

Dependency-free javascript which includes Fastave Modal into your website with minimum integration steps.
&nbsp;
### Integration

Include script before closing `</body>`:
```html
<script src="https://fastave.com/fv-modal.min.js"></script>
```

Create New FvModal Instance. Assigning instance to variable is optional:
```html
<script>
const modal = new FvModal();
</script>
```

Add data-attributes `data-fvm-open` to the elements which supposed to open modal on your website:
```html
<button type="button" data-fvm-open>Action</button>
<a href="#" data-fvm-open>Action</a>
<div data-fvm-open>Action</div>
```


Provide unique links as value for `data-fvm-open` attribute if needed. otherwise default will be used (https://www.fastave.com/):
```html
<!--with unique link-->
<button type="button" data-fvm-open="https://www.fastave.com/#/INFOGRAPHIC?dealerID=MP13422&sku=18984">Action</button>
<!--default link will be used-->
<a href="#" data-fvm-open>Action</a>
```

##### Enjoy FvModal.js!
&nbsp;
## Options
Default Options:
```html
<script>
new FvModal({
                openTriggerName = 'data-fvm-open',
                selfCloseTriggerName = 'data-fvm-self-close',
                appendToElem = document.body
            });
</script>
```

**openTriggerName** (String) - data-attribute name of the element clicking on which will open Fastave Modal.

**selfCloseTriggerName** (String) - data-attribute name of the modal child elements clicking on which will close Fastave Modal.

**appendToElem** (HTMLElement) - element in the end of which Fastave Modal will be appended.
