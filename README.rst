3Di documentation
=================

Let's try to do it with restructuredtext/sphinx!

The documentation (open source!) is automatically build on
http://3di-documentation.readthedocs.io, we can change the URL later on.


Local setup
-----------

If you can run docker, you're in luck. One-time setup::

  $ docker-compose build

And then every time you want to re-generate your documentation::

  $ docker-compose build

If you're not so lucky, you'll need to pip-install sphinx and you need latex
(see the `Dockerfile` for the short list of packages that we install).


Special commands
----------------

If the sphinx documentation tells you about a makefile: you can run those
commands from within docker, too. For example::

  $ docker-compose run builder make latexpdf


Some sphinx/restructuredtext notes
----------------------------------

You'll need to learn a bit of restructuredtext:
http://www.sphinx-doc.org/en/stable/rest.html

Special stuff, cross-references, indices etc:
http://www.sphinx-doc.org/en/stable/markup/index.html

Math support ("it is all LaTeX"):
http://www.sphinx-doc.org/en/stable/ext/math.html


Any questions: ask Reinout.
