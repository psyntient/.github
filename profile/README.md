# Psyntient

**Psyntient** is the platform: accounts, billing, the Node, Cortex, and the identity
provider at [psyntient.io](https://psyntient.io).

**The Noetic Archive** is the system it hosts at
[archive.psyntient.io](https://archive.psyntient.io) — a repository of paired
first-person reports and neural recordings, and an agent that derives a taxonomy of
experience from them.

The Repo, the Library, the Node API and the Architect are **components of the Noetic
Archive**, not peers of it. Some are named for the platform; that is a naming
accident, not a hierarchy.

---

## If you are here to restore or rebuild the droplet

**Start at [psyntient-droplet](https://github.com/psyntient/psyntient-droplet).**
Clone it and read `RESTORE.md`. It is written for whoever — or whatever — is doing
the rebuild: it names every other repository to clone, where each one deploys, which
service runs it, what cannot come from GitHub at all, and what to ask a human to get
from Lovable.

You do not need to know anything else first. That one repository is the map.

---

## What is where

| repository | what it holds |
|---|---|
| **[psyntient-droplet](https://github.com/psyntient/psyntient-droplet)** | **the map.** How the parts fit, how to rebuild, plus the auth shim, the Librarian and Cortex workspaces, and the service definitions |
| [The-Architect](https://github.com/psyntient/The-Architect) | the Architect agent **and the Archive itself** — observation packets, archetypes, methodology, pipeline tools |
| [The-Repo](https://github.com/psyntient/The-Repo) | deposit and browse surface |
| [The-Library](https://github.com/psyntient/The-Library) | the Taxonomy reading surface |
| [noetic-api](https://github.com/psyntient/noetic-api) | Node API backend and Edition build tooling |
| [The-Noetic-Archive](https://github.com/psyntient/The-Noetic-Archive) | published Editions, frozen |
| [Psyntient-Node](https://github.com/psyntient/Psyntient-Node) | the researcher's local instrument |
| [Psyntient-Installer](https://github.com/psyntient/Psyntient-Installer) | Node installers |
| [noetic-archive-reports](https://github.com/psyntient/noetic-archive-reports) | the report series |

---

*The Archive grows one consented observation at a time.*
