TODO
====

* Limit items by number or maybe better age
* Refetch already cached stuff automatically again in intervals.
  * Should default to value given in feed itself
* Access control (based on clients, feed URLs or maybe login)
* Logging

Ideas
=====

* Dynamic intervals based on request frequency
* Maybe only return cached stuff on too frequent requests
* Filtering feeds by item properties, e.g. "$feed->remove_item('');"
  filters empty LOTD items in the UF feed.
  * Needs to be configurable via configuration files
