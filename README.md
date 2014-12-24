[![Bower version](http://img.shields.io/bower/v/selection-listener.svg)](https://github.com/jbrudvik/selection-listener)

  - [SelectionListener()](#selectionlistener)
  - [SelectionListener.handleEvent()](#selectionlistenerhandleevent)
  - [SelectionListener.start()](#selectionlistenerstart)
  - [SelectionListener.stop()](#selectionlistenerstop)
  - [SelectionListener.toggle()](#selectionlistenertoggle)

## SelectionListener()

  An object that listens for selection changes on a target object and triggers
  a custom jQuery `selectionChange` event when changes are observed.
  
  Observes changes using EquatableSelection.
  
  Triggered `selectionChange` events contain a `selection` property containing an
  EquatableSelection if a selection exists. In the case of a previously-selected
  selection being unselected, the triggered `selectionChange` event will not contain
  a `selection` property.

## SelectionListener.handleEvent()

  Handle events and check for selection changes.
  
  Trigger `selectionChange` event if a selection change has occurred.
  
  `selectionChange` event includes EquatableSelection `selection` property.

## SelectionListener.start()

  Start listening for selection changes.
  
  If there is an existing selection when this method is called, a
  `selectionChange` event will be immediately triggered.

## SelectionListener.stop()

  Stop listening for selection changes.
  
  One empty `selectionChange` event is immediately triggered.

## SelectionListener.toggle()

  Toggle listening for selection changes.

# Generating documentation

    $ npm install -g dox
    $ ./generate-docs
