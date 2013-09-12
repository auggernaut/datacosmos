# DataCosmos

DataCosmos is an architecture that fosters a respectful and sustainable user/developer
relationship by separating applications from data.

An ecosystem of apps and user data stores built on DataCosmos would reduce the entry barrier
for application developers while giving more control to users.

## Design Goals

* Applications know as little as necessary about users.
* Personal data (passwords, preferences, app data) are stored locally and synced with personal servers.
* Loosely coupled services.
* Developers control access to their app.
* Users control access to their data.
* Apps work well offline.


## Overview

The DataCosmos system consists of three types of servers:

1. Nexus - Federated directory of Stars.
2. Star - Personal data storage and access control.
3. Belt - Connectors to other services.


### Nexus

A federated Star directory service.

Nexus stores the minimum necessary information about users so that their Stars can be located.

Functions:

* connecting users/apps to Stars
* Star lookup



### Star

Stars represent users in the digital world.
Stars house application data and control access to that data.
One Star can support multiple users and apps.

Functions:

* persisting user data (dust)
* managing access to dust




### Belt

Belts are the connective tissue between various services and user data stores.
These servers maintain secret keys, pass auth tokens, etc.

Functions:

* service connector




## Flows

Example DataCosmos [flows].

[flows]: https://github.com/auggernaut/datacosmos/blob/master/Flows.md