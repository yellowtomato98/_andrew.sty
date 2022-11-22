# _andrew.sty
My general use latex style file. Stylistic inspiration for this design came from some combination of the notes of [Rachel Wu](https://people.csail.mit.edu/rmwu/notes.html), [Andrew Lin](http://www.mit.edu/~lindrew/notes.html), and [Evan Chen](https://web.evanchen.cc/coursework.html). See the MWE in this repository for a fast way to set up. 

## features

* support for color boxes, as usual for most handouts. the specific color palette is viewable inside of ```_andrew.sty```.
* templates, including common matrix patterns (and block matrices), basic asymptote visuals, and table patters. useful for copy-pasting when taking notes in real-time
* support for importing lots of files. when taking notes for various classes, I usually like to organize notes by lecture in different files (e.g., 0527.tex). instead of having ```main.tex``` look like this: 
```tex
% ...
\include{0527.tex}
\include{0603.tex}
\include{0610.tex}
\include{0617.tex}
\include{0624.tex}
\include{0701.tex}
\include{0708.tex}
\include{0715.tex}
\include{0722.tex}
% ...
```
the command ```\importfiles``` does everything for you. I made this command after realizing halfway through the semester that more than 75% of my ```main.tex``` was just importing files, and it was a bit of a hassle to have to scroll all the time.

## features I want to add 
* support for theorem/corollary/proposition/etc. referencing tags