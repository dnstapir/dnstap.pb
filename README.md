# dnstap: flexible, structured event replication format for DNS software

This directory contains only the protobuf schemas for [dnstap](http://dnstap.info/), and is the root of
a repository named "dnstap.pb".

See the following repositories/links for implementations:
- [golang-dnstap](https://github.com/dnstap/golang-dnstap): command-line tool and Golang package

# Community

There is a [mailing list](http://lists.redbarn.org/mailman/listinfo/dnstap) for everyone interested in discussing `dnstap`.

# DNS TAPIR fork

The complexity of logging DNS is growing, with new transports, encryption, protocol extensions, filtering, and not least the need for exposing internal server state. This modification is an attempt at creating a true "hot potato" handling of data, where the need for carrying persistent state throughout the query session is minimized.

## Key changes:

### Adding a required session identifier

### The data from the DNS server is transmitted in a single data structure

### The approach within the server is to send partial messages whenever the data is available
