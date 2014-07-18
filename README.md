NetSNMP-agent
=============

*An extension of perl [NetSNMP::agent](http://search.cpan.org/~hardaker/NetSNMP-agent/agent.pm) module with context support*


Manual
------
Everything is similar to the original NetSNP::agent on CPAN, except the following:

###register() method

    register (NAME, OID, \&handler_routine, context)
Registers the callback handler with given OID *in the given context*. If not provided, the default context, '', is used.
