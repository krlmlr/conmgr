# conmgr

![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)

Managing database (and other) connections:

- Listens to "connect", "disconnect" and other events from packages that provide browseable connections to data objects (_DBI_ backends, ...).
- Sends out notifications to clients who wish to be notified of new/changed connections
- Returns the list of known connections upon request
- Knows/memoizes how to recreate a connection in a fresh R session
