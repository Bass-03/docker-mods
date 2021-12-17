# rbenv - Docker mod for code-server

This mod adds a rbenv to code-server, to be installed/updated during container start.

Benefit over installing a single ruby version?
`rbenv` installs shims in the home folder, hence all packages and shims will have persistence.

In code-server docker arguments, set an environment variable `DOCKER_MODS=linuxserver/mods:code-server-rbenv`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=linuxserver/mods:code-server-rbenv|linuxserver/mods:code-server-mod2`
