# kz

Kustomize version management

## Installation

```
curl -L https://raw.githubusercontent.com/corrupt952/kz/main/bin/kz -o kz
chmod u+x kz
mv kz /path/to/bin
```

`kz` command downloads and installs to /usr/local by default, but you may override this location by defining KZ_PREFIX.

```sh
export KZ_PREFIX=$HOME/.cache/kz
export PATH=$KZ_PREFIX/bin:$PATH
```

## Commands

### kz install

Download and install a version of Kustomize. If `<version>` has already been downloaded, `kz` will install from its cache.

```sh
kz install v4.4.0
```

### kz use

TBD

```sh
kz use v3.9.3 # $KZ_PREFIX/bin/kustomize version => v3.9.3

kz use v4.4.0 # $KZ_PREFIX/bin/kustomize version => v4.4.0
```

### kz exec

TBD

```sh
kz exec v3.9.3 build webapp/
```
