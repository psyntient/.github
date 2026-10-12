# Psyntient

**Psyntient** is the platform: accounts, billing, the Node, Cortex, Psyntient Cloud,
and the identity provider at [psyntient.io](https://psyntient.io).

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

## If you are here to understand Psyntient Cloud

**Start at [psyntient-cloud](https://github.com/psyntient/psyntient-cloud).** Its
`README.md` is the map: the two kinds of droplet, what a tenant is, how an instance
is built from a golden image, and the one channel the Archive has into a
researcher's machine.

Cloud is the hosted form of Cortex — one researcher, one droplet, one gateway, one
agent. It is **not** multi-tenant, and nothing is shared between researchers except
the Archive they both deposit into. The provisioning *logic* lives in
[The-Repo](https://github.com/psyntient/The-Repo) rather than in the Cloud repo,
because it runs as part of the Archive; the Cloud map says which file does what.

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
| **[psyntient-cloud](https://github.com/psyntient/psyntient-cloud)** | **the Cloud map**, plus the gateway plugin, Cortex's workspace, the Archive's Caddyfile and the provisioning scripts |
| [Open-Claw-Forked](https://github.com/psyntient/Open-Claw-Forked) | **the OpenClaw fork we actually run** — on branch **`psyntient`**, not on `main`. See the warning below |
| [openclaw-mirror](https://github.com/psyntient/openclaw-mirror) | a pinned-commit backup of upstream `openclaw/openclaw`. Not ours, not modified, kept so an upstream disappearance is survivable |
| ~~OpenClaw-Fork~~ | **superseded and empty.** An earlier fork attempt with no branches and no content. Ignore it |

---

## One trap, named here because it has no other home

[Open-Claw-Forked](https://github.com/psyntient/Open-Claw-Forked)'s **default branch
is `main`, which is upstream OpenClaw** — upstream's README, upstream's badges,
upstream's code. Every Psyntient change is on the **`psyntient`** branch. Anyone or
anything landing on that repository without switching branches will read it as
upstream's project and conclude the fork does not exist.

The branch carries `PSYNTIENT.md` at the root, which says what the fork changes and
why. Read that before reading the code.

---

*The Archive grows one consented observation at a time.*
