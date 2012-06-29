CacheCore
=========

Simple cache backends, inspired by werkzeug.contrib.cache.

Supports: 

- In-Memory
- Redis
- Memcache
- Filesystem
- Your own (extend BaseCache)

Creating a Cache Object
-----------------------

To create a cache object you just import the cache system of your choice
from the cache module and instantiate it.  Then you can start working
with that object::

    >>> from cachecore import SimpleCache
    >>> c = SimpleCache()
    >>> c.set("foo", "value")
    >>> c.get("foo")
    'value'
    >>> c.get("missing") is None
    True


Installation
------------

Installing cachecore is simple with pip::

    $ pip install cachecore