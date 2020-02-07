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

This contradicts "best practice," but perhaps for a good reason.
--
# So what is it?
Here's a basic example
~~~html
<style type="text/css">
.box {
    width: 250px;
    margin: 0 auto;
    padding-left: 2em;
}
</style>
<body>
    <div class="box">
        <p>Some stuff in dis' box.</p>
    </div>
</body>
~~~

--
# But now with ACSS
~~~html
<style type="text/css">
.w250 { width: 250px; }
.cen { margin: 0 auto; }
.pl-2 { padding-left: 2em; }
</style>
<body>
    <div class="w250 cen pl-2">
        <p>Some stuff in dis' box.</p>
    </div>
</body>
~~~

--
# WHAT!?
![Mother of god...](img/mother-of-god.jpg)


--
# Why is this useful?
* Nothing is contextual
 * No specificity issues
 * Very modular
* Portable
* With large projects, it's ultimately less CSS
* Better caching
* Only need to look in HTML for what the block does, assuming a solid naming convention.

--
# What's wrong with it?
* Responsive design is more difficult
* Since bloat doesn't exist in CSS, it naturally falls on HTML.

--
# Not convinced?
Understandbly so.  This is certainly a new CSS model and this is clearly more suited towards very big projects.

However, it's worth keeping in mind as part of your toolbelt considering the variability of web projects.  Which
leads to our next point...