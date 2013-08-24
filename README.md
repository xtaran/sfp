Semantic Feed Proxy
===================

Idea
----

Some RSS/RDF/Atom feeds contain only few items which rotate out quite
quickly. A very extrem example is
[UserFriendly's feed](http://www.userfriendly.org/rss/uf.rss) which
only contains one (relevant) item and changes every day.

To follow them my feed reader would need to fetch them at
least once a day. But my feed reader does not run if I'm
e.g. travelling and I still don't want to not miss any entry.

So I need a proxy which does not cache feeds on a per file base but on
a per item base.

Current State
-------------

As of now this is a working prototype **without**

* Cache expiration
* Limiting the amount of cached items
* Access control

Default port is 65261 (aka 0xFEED).

Requirements
------------

### Hard requirments

* Perl 5.10
* Modern::Perl
* HTTP::Proxy
* XML::FeedPP
* File::Basename
* File::Path

### Current requirements, to be discussed

* Config::IniHash

Copyright
---------

Copyright 2013 Axel Beckert <abe@deuxchevaux.org>

License
-------

This program is free software: you can redistribute it and/or modify
it under the terms of the
[GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0)
as published by the Free Software Foundation, either version 3 of the
License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but
*without any warranty*; without even the implied warranty of
*merchantability or fitness for a particular purpose*.  See the
[GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0)
for more details.
