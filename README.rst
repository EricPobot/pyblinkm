========
PyBlinkM
========

Drive a `BlinkM <http://thingm.com/products/blinkm>`_ with **Python** via I2C using python-smbus on `Raspberry Pi <http://www.raspberrypi.org/>`_.

You can view the documentation `on readthedocs <https://pyblinkm.readthedocs.org/en/latest/>`_.

Overview
========

::

    $ sudo apt-get install python-smbus
    $ sudo pip install pyblinkm
    $ python
    >>> from pyblinkm import BlinkM, Scripts
    >>> blinkm = BlinkM()
    >>> blinkm.reset()
    >>> blinkm.play_script(Scripts.THUNDERSTORM)
    >>> blinkm.reset()
    >>> blinkm.fade_to(255, 0, 0)
    >>> blinkm.fade_to_hex("ff0000")
    >>> blinkm.go_to(0, 255, 0)


Requirements
============

You must install **python-smbus** with your package manager since it is not available on pypi.

::

    $ sudo apt-get install python-smbus



Installation
============

::

    $ pip install pyblinkm



License (MIT)
=============

Copyright (c) 2012 Thomas Sileo

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
