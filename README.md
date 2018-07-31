# epics_manifest

This repository works with epics_builder [1].

## Repo

```
mkdir -p ~/bin
export PATH=~/bin:$PATH
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```


## Init

* Create the working directory
```
mkdir epics_env
cd epics_env
```

* Initialize epics_env to use the default.xml on the master branch

```
repo init -u https://github.com/jeonghanlee/epics_manifest.git
```


* Initialize epics_env to use the 1808.xml, on the master branch
```
repo init -u https://github.com/jeonghanlee/epics_manifest.git -m epics_1808.xml
```


* Sync
```
repo sync --no-clone-bundle
```
* Force Sync
```
repo sync --force-sync --no-clone-bundle
```


## epics_builder

```
$ make init
$ make base
$ make modules
```

## References
[1] https://github.com/jeonghanlee/epics_builder