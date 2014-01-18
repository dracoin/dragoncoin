Dragoncoin integration/staging tree
================================

http://www.DragonCoin.net

Copyright (c) 2009-2013 Bitcoin Developers<br>
Copyright (c) 2011-2013 Litecoin Developers<br>
Copyright (c) 2013-204 Dragoncoin Developers

What is Dragoncoin?
----------------

Dragoncoin is a derivative of Litecoin with these specifications:
 - Approximately 4-minute block targets
 - subsidy halves in 505050 blocks (~4 years)
 - 88,888,888 total coins - Eighty Eight Million Eight Hundred Eighty Eight Thousand Eight Hundred Eighty Eight!

Initialization period (first 4 years):
 - 88 coins per block
 - 8 hours to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Dragoncoin client sofware, see http://www.dragoncoin.net.

License
-------

Dragoncoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers would work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Litecoin.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake DRAGONCOIN_QT_TEST=1 -o Makefile.test dragoncoin-qt.pro
    make -f Makefile.test
    ./dragoncoin-qt_test

