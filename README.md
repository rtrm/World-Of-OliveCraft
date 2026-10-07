# World Of OliveCraft

Personal additions to vanilla World of Warcraft 1.12, built on the same client + server fork architecture as [benilla-pets-mounts-tab](https://github.com/rtrm/benilla-pets-mounts-tab). Unlike that repo, this one's scope is intentionally open-ended - a running personal server that grows feature by feature, rather than a finished, frozen project.

## Repo layout

- [`client/`](client) — [rtrm/benilla-olivecraft](https://github.com/rtrm/benilla-olivecraft), git submodule, branch `main`. A merge of two forks of [benilla](https://github.com/samwhosung/benilla):
  - [rtrm/benilla](https://github.com/rtrm/benilla) — the pets-mounts-tab client (companion pet and mount collections)
  - [pkuzic/benilla-everwood_graphics](https://github.com/pkuzic/benilla-everwood_graphics) — a graphical overhaul fork
- [`server/`](server) — [rtrm/core](https://github.com/rtrm/core) (fork of [vMaNGOS](https://github.com/vmangos/core)), git submodule, branch `development`. Already carries the pets/mounts SQL migrations; no server-side change was needed for the graphics merge, since that fork is client-only.

## Getting started

Clone with submodules:

```
git clone --recurse-submodules https://github.com/rtrm/World-Of-OliveCraft.git
```

Build instructions for the client and server live in their own READMEs ([client/README.md](client/README.md), [server/README.md](server/README.md)) — this repo only tracks the integration work on top of them.
