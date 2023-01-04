## Overview

## Testing configuration

## e2e testing

## Unit testing

### newSpecPage function 

components: [CompA, CompB]
returns a page object that has following properties:
- win: window
- doc: document
- root: top level component; HTML element of HTML created inside mockWindow
- rootInstance: class instance

page object also has some important methods:
- setContent
- waitForChanges

- exists  toBeTruthy()
- page.waitForChanges(); trigger changes on the spec page
