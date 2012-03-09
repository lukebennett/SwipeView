SwipeView v0.12 - 2011-12-17
============================

Virtually infinite loop-able horizontal carousel for mobile webkit (in 4kb).

Read more at [cubiq.org](http://cubiq.org/swipeview)

Gallery Demo: [http://cubiq.org/dropbox/SwipeView/demo/gallery](http://cubiq.org/dropbox/SwipeView/demo/gallery)

eReader Demo: [http://cubiq.org/dropbox/SwipeView/demo/ereader](http://cubiq.org/dropbox/SwipeView/demo/ereader)

Inline Demo: [http://cubiq.org/dropbox/SwipeView/demo/inline](http://cubiq.org/dropbox/SwipeView/demo/inline)

Screencast: [http://www.youtube.com/watch?v=Hhes5JHs8jQ](http://www.youtube.com/watch?v=Hhes5JHs8jQ)


Additions to cubiq's version
============================

 * the proprietary transition code for webkit has been extended to cover other browsers supporting them as well.
 * the carousel now also has a property onClick that will be fired when the control is touched, but no distance is traveled.

Usage:
    
	carousel.onClick( function() {
		alert( "clicked!" );
	} );

 * a global `active_SwipeView` is exposed to be able to nest SwipeViews in SwipeViews and avoid triggering swipes on more than.
 * a new option `handleMouseSwiping` can be set when constructing a new SwipeView object. It defines whether or not mouse swiping should be enabled. Especially when there are native elements (select boxes f.e.) it can happen that dragstart is triggered, producing wierd results.
