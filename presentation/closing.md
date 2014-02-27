# Methodology
## Which one should I choose?

---
# None or All
Your choice in front-end architecture ALWAYS depends on the scale of the project
as well as the time you have available.  

I highly encourage you to explore all of these options and either choose one, or 
combine all of them into your own architecture.  The way we use CSS is still evolving
every day, so settling on method may be narrow-minded.

---
# Which do I use?
I try to use a combination of all of them.  I primarily use OOCSS in it's ideas, but
I use a spin-off of BEM for naming purposes.  

~~~css
/* BEM */
.blockname--child__active {}

/* Me */
.blockName-child_active {}

/* Or Even */
.nameSpace-blockName-child_active {}
~~~

My choice always varies depending on the project at hand.

---
# Closing
If you're implementing a small blog site or static site that will most likely never 
change, you probably never have to deal with these methodologies.

But if you work on any project that has the potential to grow, it's imperative that
you write your CSS with granularity and modularity in mind.

---
# Pre-processors
Due to the nature of this presentation, I did not include CSS preprocessors.

However, consider looking into CSS pre-processors such as SASS or LESS.  
These preprocessors make it much easier to create stylesheets that 
follow these architectures.

---
# Sources

* OOCSS
 * [OOCSS Wiki](https://github.com/stubbornella/oocss/wiki)
 * [Article by Louis Lazaris](http://coding.smashingmagazine.com/2011/12/12/an-introduction-to-object-oriented-css-oocss/)
* SMACSS
 * [SMACSS Homepage](http://smacss.com/)
* BEM
 * [BEM Homepage](http://bem.info/)
 * [Article by Harry Roberts](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/)
* ACSS
 * [Article by Thierry Koblentz](http://coding.smashingmagazine.com/2013/10/21/challenging-css-best-practices-atomic-approach/)
* Jim Rice's personal photo collection
 * Thanks Jim!  Jim is much cooler than me.
 
---
# Questions?

---
# Thank you!