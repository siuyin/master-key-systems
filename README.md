# Master Key or Key Encryption Key generation

Generating a master key is similar to a
multi-factor authentication exercise.

The "user" to be authenticated is the
system which is secured by the master key.

The System runs a master key vault (MKV)
program. This program _knows_ something
about the System.

The System must _have_ some files and
timestamps.

Finally the program check features
of what the system _is_. Features
such as CPUID, network card MAC address
and/or filesystem UUID.

The combination of all the above factors
is used to generate the master key.

Note: mmd files are mermaid files.
Render with https://github.com/mermaid-js/mermaid-live-editor .
