Semantic Feed Proxy
===================

Idea
----

Some RSS/RDF/Atom feeds contain only few items which rotate out quite
quickly. A very extrem example is UserFriendly's feed which only
contains one (relevant) item and changes every day.

To follow them my feed reader would need to fetch them at
least once a day. But my feed reader does not run if I'm
e.g. travelling and I still don't want to not miss any entry.

So I need a proxy which does not cache feeds on a per file base but on
a per item base.

Current State
-------------

As of now this is just a proof of concept with a hardcoded feed
(UF's).
