Spin
===========

This is a port of jQuery Orbit

![Screenshot](http://w857226.open.ge.tt/1/files/89QVUSH/0/blob/x675?noinc=1)

How to use
----------

<script type="text/javascript">
     window.addEvent("domready", function() {
         $('#featured').spin();
     });
</script>

or advanced use

<script type="text/javascript">
     window.addEvent("domready", function() {
         $('#featured').spin({
			transition: "horizontal-push",//fade, horizontal-slide, vertical-slide, horizontal-push
			transitionOption: {transition:"linear",duration:600},
			timer: true,// true or false to have the timer
			advanceSpeed: 4000,// if timer is enabled, time between transitions
			pauseOnHover: false,// if you hover pauses the slider
			startClockOnMouseOut: true,// if clock should start on MouseOut
			startClockOnMouseOutAfter: 1000,// how long after MouseOut should the timer start again
			directionalNav: true,// manual advancing directional navs
			captions: true,// do you want captions?
			captionTransition: "fade",//fade, slideOpenH , slideOpenV, followSlide,none
			captionTransitionOption: {transition:"linear",duration:600},// fade, slideOpen, none
			bullets: true,// true or false to activate the bullet navigation
			bulletThumbs: false,// thumbnails for the bullets
			bulletThumbLocation: '',// location from this file where thumbs will be
			afterSlideChange: function(){}// empty function
		});
     });
</script>

<div id="featured"> 
        <div class="content" style="">
                <h1>Orbit does content now.</h1>
                <h3>Highlight me...I'm text.</h3>
        </div>
        <a href=""><img src="dummy-images/overflow.jpg" /></a>
        <img src="dummy-images/captions.jpg" data-caption="#htmlCaption" />
        <img src="dummy-images/features.jpg"  />
</div>