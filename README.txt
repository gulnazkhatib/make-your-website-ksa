Make My Website KSA
@gulnazkhatib
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)


So I've been on a single page kick as of late, partly because I'm lazy, but
mostly because they are great for experimentation. In this case, it
makes heavy use of my (tentatively named and soon to be released) "scrollgress"
and "scrollwatch" jQuery plugins to pull off some interesting effects as you
scroll around the page. In addition to said interesting effects, Big Picture
also includes a nice lightbox-style gallery, styling for basic page elements,
and thoroughly commented code for your editing pleasure (with instructions!
-- see below).


PS: Not sure how to get that contact form working? Give formspree.io a try (it's awesome).


Instructions:

	Overview:

		Being a single pager, Big Picture should be way simpler to work with than
		some of the heavier stuff I've released in the past. In fact, aside from
		a main page <header> and <footer>, it's pretty much just a stack of "main"
		<section> elements that follow the same basic pattern:

			<section id="foobar" class="main">
				<div class="content container">
					<header>
						<h2>Foobar</h2>
					</header>
					...
				</div>
			</section>

		The section can then be assigned a style class to determine its basic
		look (and, in some cases, its behavior):

			style1
				Centered content with an oversized <h2>. Works best when
				paired with a background image or color.

			style2 left
				Content in a box, anchored to the left side of the window. Works
				best when paired with a background image or color. If you have
				"useSectionTransitions" turned on in your settings, the box will
				slide into view from the left.

			style2 right
				Content in a box, anchored to the right side of the window. Works
				best when paired with a background image or color. If you have
				"useSectionTransitions" turned on in your settings, the box will
				slide into view from the right.

			style3 primary
				Used for generic content. Set against the primary background
				color (default is white).

			style3 secondary
				Used for generic content. Set against the secondary background
				color (default is a light gray).

		Oh, and there are a few (well, two) optional modifier classes you can
		tack on for additional effects:

			dark
				Flips the content's color scheme so it shows up better
				against darker background images and colors.

			fullscreen
				Makes the section fill the entire window (only if "useFullScreen"
				is enabled in your settings).


	Lightbox Gallery:

 		The actual gallery function is powered by my Poptrox plugin. For info on
 		how that works, go here: github.com/ajlkn/jquery.poptrox

		Each image (the '...' bit in the above examples) should look like this:

			<article class="from-(direction)">
				<a href="path/to/fullsize.jpg" class="image fit">
					<img src="path/to/thumbnail.jpg" title="This is the image caption." alt="" />
				</a>
			</article>

		The "from-(direction)" class indicates the direction from which the image should
		slide into view, and can be any of the following:

			from-left
			from-right
			from-bottom
			from-left

		You can also just remove the "from-(direction)" class if you don't want that particular
		image to slide into view (in which case it'll simply fade in).


	Contact Form:

		To get this working, place a script on your server to receive the form data, then
		point the "action" attribute to it (eg. action="http://mydomain.tld/mail.php").
		More on how it all works here: 1stwebdesigner.com/tutorials/custom-php-contact-forms


