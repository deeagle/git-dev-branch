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

## Mhhhh

Not the nicest git-graph:

![fazit](git-dev-branch_fazit.png)

The single branches should be updated before merging.
Steps to activate:

- Settings
- Branches
- Protection rules
- [x] Require a pull request before merging
- [x] Require status checks to pass before merging
- [x] Require branches to be up to date before merging

Further details: https://github.blog/changelog/2022-02-03-more-ways-to-keep-your-pull-request-branch-up-to-date/

-> may I must ensure this for explicit topic branches in my environments.
