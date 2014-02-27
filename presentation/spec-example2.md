# How can this get hairy?
~~~css
div#thisidname--istoolong .dang { background-color: #000; }

/* This overrides this on certain occassions: */

.dang { background-color: #00F; }

/* Wanna change it later? */

div#thisidsname--istoolong div.dang { background-color: #FFF; }
/* Or */
body div#thisidname--istoolong div.dang { background-color: #000; }
/* Etc. */
~~~
Nasty, right? Very unmanageable.
## Jim is still very, very disappoint.