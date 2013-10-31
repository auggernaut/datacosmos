# DataCosmos

DataCosmos is a reimagining of the internet using the metaphor of the cosmos.


## Overview

The DataCosmos consists of these types of objects:

1. Star - Center of a star system.
2. Dust - Small piece of metadata in a star system.
3. Planet - Large chuck of data in a star system.
4. Naut - Vessel a human uses to traverse the cosmos.
5. Nexus - Map of stars in the cosmos.



### Star

Stars are the powerhouses of the cosmos. They create immense gravity wells around which
planets and dust orbit. Stars are constantly churning, turning matter into energy and back again.
The photons of light they create travel the cosmos.
http://en.wikipedia.org/wiki/Star

A Star in the DataCosmos is a server with the following functions:

* storage - persisting data (dust and planets)
* processing - running programs
* events - communicating with other stars in the cosmos



### Dust

Dust are solid particles floating in the cosmos.
http://en.wikipedia.org/wiki/Cosmic_dust

Dust in the DataCosmos are metadata that are:

* structured - machine readable json
* content-addressable - their ids are the sha384 hash of their content
* colored - falls somewhere on the visible light spectrum.



### Planet

Planets are massive objects that orbit stars.
http://en.wikipedia.org/wiki/Planet

Planets in the DataCosmos are large binary objects that are:

* content-addressable - their ids are the sha384 hash of their content
* colored - falls somewhere on the visible light spectrum.



### Naut

Nauts are the vessels we explorers travel in i.e. our space ships.

Nauts in the DataCosmos are keys that uniquely identify a user.



### Nexus

Nexus are the maps of the stars in the cosmos. They plot where the stars are, giving us the
means to navigate the cosmos.

Nexus in the DataCosmos are directory servers for Stars.





## Flows

Example DataCosmos [flows].

[flows]: https://github.com/auggernaut/StarTier/blob/master/Flows.md