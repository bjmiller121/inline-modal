# Inline Modal jQuery Plugin

This jQuery plugin is used to display modal content on the page inline with other content. Content can be displayed in a variety of ways relative to the trigger element.

### Options
* content: $('#content')
  * jQuery object of the content to be loaded
* container: $('#container')
  * jQuery object of the container of the trigger in which to position the content relative to.
* mode: { above | *below* | overlay }'
  * Where the content should be positioned relative to the container
* animation: '{*fade* | slide | none}'
  * The animation to use when displaying the content
* animationDuration: 400
  * Duration of time the animation takes in milliseconds
* oneAtATime: false
  * Determines whether or not more than one inline modal can be expanded simultaneously.
* triggerClose: true
  * Determines whether clicking the trigger again closes the content
* closeLink: 'Close'
  * Text to use for the close link
* closePosition: '{ *above* | after | below }'
  * Location within the content pane in which to position the close link
