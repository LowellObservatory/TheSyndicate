# Python Environments

* Anaconda Python 3.6
* Miniconda Python 3.6

Q: I feel pretty strongly that self-managed (i.e. apt-get/pip or brew/pip)
   installations should be discouraged, since they can frequently be hard to
   update and maintain. What says the crowd?

C: If desired, docker images (and the associated Dockerfiles) can be provided
   to quickly jump into the "standard" Lowell software environment for
   testing/verification.  This is already being done for some new codes
   at the DCT [like the DataServants](https://github.com/LowellObservatory/DataServants).

## Built-in Libraries:

The following list is really for information only and may not include
all of the built-in libraries used.

- os
- sys
- json
- mmap
- time
- fcntl
- datetime
- xml.etree.ElementTree

## Required External Libraries:

The following libraries have been used or deemed important. Considered the
"standard set" that should be in *every* development environment.

Q: Additions and subtractions should be vetted and agreed upon by
   The Syndicate before being added to the list; is a pull request
   the easiest way to do this?

Package Name | Minimum Version | Description
-------------|-----------------|------------
numpy | | array manipulation, matrix math, algorithms, etc.
scipy | | fancier/complicated math extensions to numpy
matplotlib | | plotting
astropy | | useful astronomy stuff
ipython | | a much nicer interactive python shell
sphinx | | self-documenting code
sphinx_rtd_theme | | "Read The Docs" theme for sphinx
cython | | C extensions for python
swig | | Way to make python wrappers around ugly C
pillow | | common image (JPG/PNG/etc.) manipulations
paramiko | | wrapper for playing nicely with ssh
psutil | | various PID and process/file system utilities
pylint | | automated code checks
stomp.py | 4.1.21 | used to talk to the ActiveMQ broker (via the STOMP protocol)
xxhash | | Fast, non-cryptographic hashing
serviceping | 18.8.1 | quick and pythonic way to get ping information without screwing around with subprocess or running as root
pid | | PID files and locking to ensure only one code instance runs at a time
xmlschema | 0.9.28 | Library to parse XML into a usable object, includes validation against a given XML schema


### Optional Libraries for More Specific Use Cases

- influxdb-python: time series database
    - REQUIRES additional installation of InfluxDB binaries on system,
      but if you don't intend to use it this is fine (but non-functional) solo
- PyQt5: GUI creation and development tools
- pyserial: talk to serial devices, either directly or thru other means
  (works with network serial ports such as the MOXAs)
