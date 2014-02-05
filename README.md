Dragoncoin integration/staging tree
================================

http://www.DragonCoin.net

Copyright (c) 2009-2013 Bitcoin Developers<br>
Copyright (c) 2011-2013 Litecoin Developers<br>
Copyright (c) 2013-2014 Dragoncoin Developers

What is Dragoncoin?
----------------

Dragoncoin is a derivative of Litecoin with these specifications:
 - Network seeding is hosted at DragonCoin.info and is built into the program
 - 8,888 coins released per block
 - Approximately 4-minute block reward spacing
 - Subsidy halves in 500050 blocks (approximately 4 years)
 - Dispensing Schedule: First year = 4,444,444,444 | Second year = 2,222,222,222 | Third year = 1,111,111,111 | Fourth year = 555,555,555.5
 - Last coin to be mined will be in the year of 2066. Thereafter, transaction fees shall provide incentives for mining
 - Total coins: 8,888,888,888 - Eight Billion Eight Hundred Eighty Eight Million Eight Hundred Eighty Eight Thousand Eight Hundred Eighty Eight!

Initialization period (first 4 years):
 - 8888 coins per block
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
regularly to indicate new official, stable release versions of Dragoncoin.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake DRAGONCOIN_QT_TEST=1 -o Makefile.test dragoncoin-qt.pro
    make -f Makefile.test
    ./dragoncoin-qt_test

