Wrapper to ln that is consistent with other UNIX commands (cp, mv, scp, etc)

This is strange because `ln FROM TO` is not consistent with mv or copy, in my mind at least. That would mean the first arg is created and the second arg must already exist -- not the case for cp mv or scp.

So instead think of it as `ln REAL LINK`

You can pass opts at the end (such as -s) but thats support is pretty lame at the moment.

ERROR CODES:
1 - no REAL specified
2 - no LINK specified
3 - REAL does not yet exist
4 - LINK already exists

Plus prints a friendly message.

Enjoy!
