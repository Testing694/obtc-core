oBTC Core integration/staging tree
=====================================

https://powx.org

What is Optical Bitcoin (oBTC)?
-------------------------------

oBTC is a fork of Bitcoin aiming to reduce mining energy consumption via compatability with cutting edge optical compute cores.  Like
Bitcoin, oBTC is an experimental digital currency that enables instant payments
to anyone, anywhere in the world. oBTC uses peer-to-peer technology to
operate with no central authority: managing transactions and issuing money are
carried out collectively by the network. oBTC Core is the name of open
source software which enables the use of this currency.

For more information, as well as an immediately usable, binary version of
the Bitcoin Core software, see https://powx.org/, or read the
[Towards Optical Proof of Work Manuscript](https://assets.pubpub.org/xi9h9rps/01581688887859.pdf).

License
-------

oBTC Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of oBTC Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

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

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.


Contributors
------------

The project would be impossible without the Bitcoin Core. We thank the Bitcoin
Core contributors for their effort.

Below is the list of people who brought the oBTC project to life.

* Mike Dubrovsky [Co-Founder]
* Roman Zhytar [SW Developer]
* Anton Kovalov [SW Developer]
* Egor Shymko [SW Developer]
* Nikita Koypish [SW Developer]
* Vsevolod Hulchuk [SW Developer]
* Mustafa Hammood [HW Prototype Developer; System]
* Jaspreet Joha [HW Prototype Developer; Simulations]
* Stephen Lin [HW Prototype Developer; Simulations]
* Sunil Kochikar Pai [HW Prototype Developer; Matrix Mult Core]
* Marshall Ball [Cryptography; HeavyHash]
* Lucianna Kiffer [Cryptoeceonomics]
* Guy Corem [Sage Advice]
* Diedrik Vermeulen [Silicon Photonics Advisor; System Architecture and Link Budgets]
* Bogdan Penkovsky [Co-Founder]

We also thank everyone who believed in us but is not on the list.
