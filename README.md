# Inline Modal jQuery Plugin

This jQuery plugin is used to reveal content on the page inline with other content. Content can be displayed in a variety of ways relative to the trigger element.

Inspiration: http://uxmovement.com/content/inline-modal-windows-display-new-content-in-page-sections/

### Better Name Ideas
* Inline Reveal
* Contextual Expander
* Inline Expand
*


### Options
* **content**: $('#content') (Required)
  * jQuery object of the content to be revealed.
* **container**: $('#container')
  * jQuery object of the container of the trigger in which to position the content relative to. Defaults to the trigger element itself.
* **mode**: [ 'above' | **'below'** | overlay ]
  * Where the content should be positioned relative to the container. Overlay will position the content over the top of the container. This requires custom CSS in order to work properly, particularly giving the overlayed content a background.
* **animation**: [ **'fade'** | slide | none ]
  * The animation to use when displaying the content.
* **animationDuration**: 400
  * Duration of time the animation takes in milliseconds.
* **oneAtATime**: false
  * Determines whether or not more than one inline modal can be expanded simultaneously. This can be useful for things like an image gallery where only one image should be expanded at a time.
* **triggerClose**: true
  * Determines whether clicking the trigger again closes the content.
* **closeLink**: 'Close'
  * Text to use for the close link.
* **closePosition**: [ **'above'** | 'below' | 'none' ]'
  * Location within the content element in which to position the close link.

### Usage
```JavaScript
$('.trigger').inlineModal({
  option: value,
});
```

### Example
```JavaScript
$('.trigger').inlineModal({
  content: $('.content'),
  container: $('.container'),
  mode: 'overlay',
  animation: 'slide',
  animationDuration: 350,
  oneAtATime: true
});
```
