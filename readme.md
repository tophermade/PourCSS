# Pour CSS
Right now just drafting out syntax ideas for a 
new css preprocessor, supporting all the stuff
missing from LESS, while trying to stay lightweight,
looking at you SASS.

## What it is
Lightweight, portable, compilable language that
generates CSS.

### Why
The major preprocessors are older, and come with 
baggage from earlier needs. Ditch the baggage, 
in with the new or something, right?

#### What it does better
Mixins are crappy, and they bloat code. Pour uses
"mixdowns" which instead of bloating the css by
dumping the same declarations all over the place,
it applies the declarations to all the selectors
on which it is placed at once.

Media queries still suck in preprocessors. There
is no immediate way to define them while in scope
in either LESS or SASS. In Pour @VALUE while in
scope will assign the declarations following to
a query with VALUE as the query rule.

##### Also
If this manages to make it beyond research, it 
will ship with cross platform compilation tools 
GUI and otherwise.

##### Caveats
Media query sorting is presently an issue for
anything other than min/max width & height.