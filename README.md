# git-dev-branch

Playground to see commit graph in real.

## To test

The following scenario:

```mermaid
gitGraph
    commit
    branch develop
    branch featA
    branch featB
    branch featC
    checkout featA
    commit
    commit
    checkout featB
    commit
    commit
    commit
    checkout featC
    commit
    commit
    commit
    commit
    checkout develop
    merge featA
    merge featB
    merge featC
    commit
    checkout main
    merge develop
    commit
    commit
```
