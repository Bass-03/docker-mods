# Pyenv - Docker mod for code-server

This mod adds a pyenv to code-server, to be installed/updated during container start.

Benefit over installing a single python version?
`Pyenv` installs shims in the home folder, hence all packages and shims will have persistence.

In code-server docker arguments, set an environment variable `DOCKER_MODS=linuxserver/mods:code-server-pyenv`

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=linuxserver/mods:code-server-pyenv|linuxserver/mods:code-server-mod2`
