# Reference

<!-- DO NOT EDIT: This document was generated by Puppet Strings -->

## Table of Contents

### Resource types

* [`host`](#host): Installs and manages host entries.

## Resource types

### <a name="host"></a>`host`

For most systems, these entries will just be in `/etc/hosts`, but some
systems (notably OS X) will have different solutions.

#### Properties

The following properties are available in the `host` type.

##### `comment`

A comment that will be attached to the line with a # character.

##### `ensure`

Valid values: `present`, `absent`

The basic property that the resource should be in.

Default value: `present`

##### `host_aliases`

Any aliases the host might have.  Multiple values must be
specified as an array.

##### `ip`

The host's IP address, IPv4 or IPv6.

##### `target`

The file in which to store service information.  Only used by
those providers that write to disk. On most systems this defaults to `/etc/hosts`.

#### Parameters

The following parameters are available in the `host` type.

* [`name`](#name)
* [`provider`](#provider)

##### <a name="name"></a>`name`

namevar

The host name.

##### <a name="provider"></a>`provider`

The specific backend to use for this `host` resource. You will seldom need to specify this --- Puppet will usually
discover the appropriate provider for your platform.

