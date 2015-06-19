Please install the repo script: http://source.android.com/source/downloading.html#installing-repo

Essentially:

```
mkdir ~/bin
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```

Then get the repos:

```
mkdir -p env/master && cd env/master
repo init -q -u https://github.com/vicenteg/ansible-repo-manifest.git -b master
repo sync -q --no-clone-bundle
```
