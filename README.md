# in-memory-cram-md5-handler-example

This repository provides source code for a sample InMemorySASLBindHandler for
the UnboundID LDAP SDK for Java's in-memory directory server.  This SASL bind
handler implements support for the CRAM-MD5 SASL mechanism.  This mechanism is
obsolete and should not be used for real-world authentication (which is why
it's not being included in the LDAP SDK itself), but the code here can be used
as a starting point for demonstrating how to create a custom
InMemorySASLBindHandler implementation for other, more desirable SASL
mechanisms (especially those that rely on the javax.security.sasl.SaslServer
class to perform the core processing).

Also see the com.unboundid.ldap.listener.PLAINBindHandler class for an example
of an InMemorySASLBindHandler that does not make use of the SaslServer
framework.
