brew-tools
==========

::

     ____  ____  ____  _  _    ____  __    __   __    ____
    (  _ \(  _ \(  __)/ )( \  (_  _)/  \  /  \ (  )  / ___)
     ) _ ( )   / ) _) \ /\ /    )( (  O )(  O )/ (_/\\___ \
    (____/(__\_)(____)(_/\_)   (__) \__/  \__/ \____/(____/

|Build Status| |Documentation Status| |PyPI version|

A command line utility that offers a set of calculators for home
brewers.

Description
===========

Need to do a quick calculation during your brew day? Don't fancy digging
through a GUI application, or a web based tool? Prefer to do simple
things in a terminal?

Then **brew-tools** is for you.

Currently brew-tools includes:

-  ABV calculator
-  Keg priming calculator
-  Priming sugar calculator
-  Quick infusion calculator

More to come

Installation
============

Brew-tools is available from PyPI

::

    pip install brew-tools

You can also clone/download this repository and install it using pip

::

    cd <brew-tools-dir>
    pip install .

Usage
=====

Brew tools has built in help

::

    Usage: brew-tools [OPTIONS] COMMAND [ARGS]...

    Options:
    --version  Show the version and exit.
    -imperial  Use imperial units. Metric by default.
    --help     Show this message and exit.

    Commands:
    abv
    infuse
    kegpsi
    prime

and also for its commands

::

    brew-tools infuse --help
    Usage: brew-tools infuse [OPTIONS]

    Options:
      -temp FLOAT    Current temperature of mash
      -target FLOAT  Target temperature of mash
      -ratio FLOAT   Grist/water ratio
      -grain FLOAT   Weight of grain in mash
      -water FLOAT   Temp of infusion water
      --help         Show this message and exit.

If the inputs are not passed via the command line arguments, brew tools
will prompt the user for input.

For more information see the
`documentation <https://brew-tools.readthedocs.io/en/latest/>`__

Development
===========

If you want to help develop brew tools you should install it into a
virtual environment.

Create and source the environment and then install brew tools with

::

    cd <brew-tools project dir>
    pip install -e ".[testing]"

which will install an editable version, as well as all the tools
required to run the tests with

::

    pytest tests

Thanks
======

Thanks to

-  /u/DAMNIT\_REZNO - for inspiring me to start this project

License
=======

Brew Tools is released under the MIT license.

See ``LICENSE.txt`` for more details

.. |Build Status| image:: https://travis-ci.com/Svenito/brew-tools.svg?branch=master
   :target: https://travis-ci.com/Svenito/brew-tools
.. |Documentation Status| image:: https://readthedocs.org/projects/brew-tools/badge/?version=latest
   :target: https://brew-tools.readthedocs.io/en/latest/?badge=latest
.. |PyPI version| image:: https://badge.fury.io/py/brew-tools.svg
   :target: https://badge.fury.io/py/brew-tools
