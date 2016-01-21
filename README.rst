PostScript Fractals
===================

There have never been more consumer-accessible CNC-like machines:

- Laser cutters / engravers
- Vinyl cutters
- 3D printers
- CNC routers
- Plasma cutters (a bit of a stretch, but check your local `makerspace <http://maker-works.com/>`_)

Many of these machines work best with vector graphics, and there are plenty of vector graphic programs for drawing things manually. But what if you want to create something intricate and repetitive, like a fractal?

Enter `PostScript <https://en.wikipedia.org/wiki/PostScript>`_, a decades-old stack-based extra-hyphenated programming language that's perfect for defining recursive fractals.

For example, take clamshell.eps. If you change the last line to be::

    500 1 DARK_TRAPAZOID

... and rendering it to a PDF (on \*nix anyways)::

    ps2pdf clamshell.eps clamshell1.pdf

... you get a small fractal:

.. image:: http://raw.github.com/steiza/postscript_fractals/master/rendered/clamshell1.png

But if you crank up the recursion by changing the last line to be::

    500 5 DARK_TRAPAZOID

... you get something much more complex:

.. image:: http://raw.github.com/steiza/postscript_fractals/master/rendered/clamshell.png

More correctly, these are actually `aperiodic tilings <https://en.wikipedia.org/wiki/Aperiodic_tiling>`_ there are built using `substitution rules <https://en.wikipedia.org/wiki/Aperiodic_tiling#Substitutions>`_, and `there are a lot of them <http://tilings.math.uni-bielefeld.de/>`_.

.. image:: http://raw.github.com/steiza/postscript_fractals/master/rendered/canonical3.png

So download this repo, make some fractals, and put them on stuff!

.. image:: http://raw.github.com/steiza/postscript_fractals/master/rendered/closet.jpg
