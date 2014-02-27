# How can this get hairy?
~~~css
div#thisclassname--istoolong .dang { background-color: #000; }

/* This overrides this on certain occassions: */

.dang { background-color: #00F; }

/* Wanna change it later? */

div#thisclassname--istoolong div.dang { background-color: #FFF; }
/* Or */
body div#thisclassname--istoolong div.dang { background-color: #000; }
/* Etc. */
~~~
Nasty, right? Very unmanageable.