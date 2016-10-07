G.729 codec wrapper
-----------------------------

This is a wrapper around the G.729 codec developed by [Belledonne
Communications](http://www.belledonne-communications.com/).

[G.729](https://en.wikipedia.org/wiki/G.729) is a widely used low-band (8khz)
codec.

How to build G.729 codec wrapper
-----------------------------

 1. Get and install Belledonne Communications [bcg729
    codec](https://github.com/BelledonneCommunications/bcg729).

 2. Build bcg729 library:

```
   configure
   make
   make install
```

 3. Build sems:

```
   cmake -DSEMS_USE_G729=yes
   make
   make install
```

 About Licensing
 ---------------

There are two distinct parts to G.729 licensing: the software licensing and the
codec (patents) licensing.

 A. Software licensing

 1. The g729 codec wrapper code is licensed under simplified BSD license (see [g729.c](./g729.c)).

   * Copyright (c) 2007, Vadim Lebedev
   * Copyright (c) 2010, Stefan Sayer
   * Copyright (c) 2012, Peter Lemenkov

 2. Belledonne Communications bcg729 codec is licensed under GPLv2 or later.

 3. SEMS is licensed under GPLv2 or later.

 B. Codec licensing

To use G.729 codec, in some countries you need to get a license to use the
patents (at least until 2016 or so). The G.729 patent pool is managed by
[Sipro](http://www.sipro.com/).
