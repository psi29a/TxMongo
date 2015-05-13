Changelog
=========

Release 15.1 (UNRELEASED)
-------------------------

This release is dedicated to fine-tuning 3.0 support.

Bugfixes
^^^^^^^^
- Use travis-ci, tox and coveralls infrastructure
- With above, we've identified a number of tests that fail.


Release 15.0 (2015-05-04)
-------------------------

This is the first release using the Twisted versioning method.

API Changes
^^^^^^^^^^^

- ``collections.index_information`` now mirrors PyMongo's method.
- ``getrequestid`` is now ``get_request_id``

Features
^^^^^^^^

- Add support for 2dsphere indexes, see http://docs.mongodb.org/manual/tutorial/build-a-2dsphere-index/
- PEP8 across files as we work through them.
- Authentication reimplemented for ConnectionPool support with multiple DBs.
- Add support for MongoDB 3.0

Bugfixes
^^^^^^^^

- Fixed failing tests due to changes in Python in 2.6
- Fixed limit not being respected, which should help performance.
- Find now closes MongoDB cursors.
- Fixed 'hint' filter to correctly serialize with double dollar signs.


Improved Documentation
^^^^^^^^^^^^^^^^^^^^^^

- Added, updated and reworked documentation using Sphinx.
- The documentation is now hosted on https://txmongo.readthedocs.org/.


Release 0.6 (2015-01-23)
------------------------

This is the last release in this version scheme, we'll be switching to the Twisted version scheme in the next release.

API Changes
^^^^^^^^^^^

- TxMongo: None

Features
^^^^^^^^

- Added SSL support using Twisted SSLContext factory
- Added "find with cursor" like pymongo
- Test coverage is now measured. We're currently at around 78%.

Bugfixes
^^^^^^^^

- Fixed import in database.py


Release 0.5 (2014-10-02)
------------------------

Code review and cleanup


Bugfixes
^^^^^^^^

 - Bug fixes


Release 0.4 (2013-01-07)
------------------------

Significant performance improvements.

API Changes
^^^^^^^^^^^

- TxMongo: None

Features
^^^^^^^^

- Support AutoReconnect to connect to fail-over master.
- Use pymongo instead of in-tree copy.

Bugfixes
^^^^^^^^

 - Bug fixes

Release 0.3 (2010-09-13)
------------------------

Initial release.

License
^^^^^^^

- Apache 2.0
