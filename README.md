WaterCoin Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/watercoin-project/watercoin.svg?branch=master)](https://travis-ci.org/watercoin-project/watercoin)

USEFUL LINKS
----------------
Website: https://wtrcoin.io/en 

Whitepaper: https://wtrcoin.io/assets/whitepaper_en.pdf 

Facebook: https://www.facebook.com/Watercoin-WTR-2144726212408130/?ref=bookmarks 

Twitter: https://twitter.com/watercoinWTR 

LinkedIn: https://www.linkedin.com/company/watercoin/ 


WALLETS
----------------

Linux QT Wallet: 
https://github.com/thewatercoin/watercoin-source/releases/download/Wallets/watercoin-qt-linux.tar.gz 

Windows QT Wallet: 
https://github.com/thewatercoin/watercoin-source/releases/download/Wallets/watercoin-qt-windows.zip  

MAC OS QT Wallet: 
https://github.com/thewatercoin/watercoin-source/releases/download/Wallets/watercoin-qt-macos.dmg 

Raspberry Pi QT Wallet: 
https://github.com/thewatercoin/watercoin-source/releases/download/Wallets/watercoin-qt-raspberry.tar.gz 


DAEMON (Windows & Linux)
----------------

https://github.com/thewatercoin/watercoin-source/releases/tag/Daemon


What is WaterCoin?
----------------
The WTR watercoin will allow O'CLAIRE, a subsidiary of SUNWATERLIFE, 
to have sufficient means to distribute its O'CLAIRE drinking water on 3 continents. 
The sums raised will be used in particular to acquire and set up drinking water production units, set up production, distribution and sales 
and marketing teams, and make the necessary communications investments to deploy the brand. 
A portion of the amounts raised will be locked in to meet sufficient financial guarantees.

What is O'CLAIRE?
----------------
O'CLAIRE, a subsidiary of SUNWATERLIFE, was created out of the desire to provide drinking water to all, at prices adapted to the populations 
of emerging areas and above all to ensure its quality and safety throughout the value chain: supply and control of production units, 
own operation with local teams, maintenance, control, testing and management. To achieve this, we pool expertise, ideas and people who have a culture 
and know-how that can make O'CLAIRE's ambition a reality: to develop a brand of drinking water in bulk and in bottles that is accessible to everyone, on 3 continents. 
Through a decentralized network of autonomous Sunwaterlife kiosks, connected locally and globally, O'CLAIRE will provide 500 million litres of drinking water per year, 
giving more than 1 million inhabitants access to quality water. Beyond the supply of drinking water, O'CLAIRE wishes to develop an ecosystem with partners providing 
related products and services, by allowing them to use the WTR watercoin, a cryptocurrency created during this ICO. Without being exhaustive, we imagine for example the 
supply of electricity (via our solar panels), the sale of ice cubes, the sale of syrups, the charging of mobile phones...

For more information, as well as an immediately useable, binary version of
the WaterCoin Core software, see [https://wtrcoin.io/en](https://wtrcoin.io/en).

License
-------

WaterCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/watercoin-project/watercoin/tags) are created
regularly to indicate new official, stable release versions of WaterCoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/watercoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #watercoin-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to WaterCoin periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
