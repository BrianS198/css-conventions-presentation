# ACSS
* "Atomic CSS"
* Made by I have no idea who the hell did this.  Probably Jim Rice.
* Methodology
* Well-known article is available [here.](http://coding.smashingmagazine.com/2013/10/21/challenging-css-best-practices-atomic-approach/)

--
# Controversy
Before getting too involved in ACSS, know that this method will certainly challenge everything
that you've most likely used in the past with CSS.

--
# So what is it?
The controversy is...

<img class="fragment right jim" data-fragment-index="1" src="img/jim-right.png">
<h2 class="fragment" data-fragment-index="1">JAMES "JIMMY" RICE!  *GASP*</h2>

--
# Okay..
Sorry, I'll use fewer Jim Rice jokes.  

Anyway, ACSS puts most of the styling onus on the markup as opposed to the CSS so
it's actually more similar to inline styling than it is traditional CSS.
--
# Refactor
Now you use this instead:
~~~css
.wrap {
	width: 960px;
	margin: 0 auto;
	background: #FFF;
}

.header {
	padding: 2em;
	border-bottom: solid 1px #000;
	color: #EEE;
}

.content { box-shadow: 0 0 20px #888; }

.footer {
	position: relative;
	border-top: solid 1px #000;
}
~~~
Because wrap is consistently used, it's declared separately as a "skin."
Want to change the width of your content?  It's one place.

--
# Separate structure and skin cont.
This also entails styling class names over elements, e.g.:
~~~css
.img { }
/* VS */
img { }
~~~
According to Nicole, what if an arbitrary tag replaces img?  Using a class name rather than 
the element name helps speed up development times for future updates.

--
# Separate container and content
<div class="grid">
	<div class="col-1-2">
		<p>But, Brian, what is this?</p>
	</div>
	<div class="col-1-2">
		<div class="fragment roll-in" data-fragment-index="1">
			<img class="jim _is-confused" src="img/jim-confused.png">
			<h2>Jim is confoosed</h2>
		</div>
	</div>
</div>

--
# This means..
Avoid using location-dependent styles.  You essentially want all of your objects looking the same
no matter where you place them.

--
# Example
Let's say you have a comment inside of a wrapper.
~~~css
/* BAD */
.wrapper p { 
	color: #FFF;
	-webkit-animation: blink 1s steps(1,end) 0s infinite; /* Because they took our tag away... */
}
/* GOOD */
.comment {
	color: #FFF;
	-webkit-animation: blink 1s steps(1,end) 0s infinite; /* Because they took our tag away... */
}
~~~

--
# Using this principle

1. All unclassed paragraph tags will look the same.
2. All '.comment' classes will look the same regardless of element.
3. If you wanted '.wrapper p' to be different than the above style for one particular object, you wouldn't have to create an override style.

--
# Sweet, right?
If you like this particular method, I urge you to read more about Nicole's 'media' object
as well as some other successful implementations of OOCSS.