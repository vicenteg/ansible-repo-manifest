Prereqs
====

You'll need to have installed git, and configured it with `git config --global user.email <you@domain.com>` and `git config --global user.name "Your Name"`.


Installing
====

Please install the repo script: http://source.android.com/source/downloading.html#installing-repo

Essentially:

```
mkdir ~/bin
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```

Then get the repos:

```
mkdir -p env/mapr-hbindexer && cd env/mapr-hbindexer
~/bin/repo init -q -u https://github.com/vicenteg/ansible-repo-manifest.git -b hbindexer
~/bin/repo sync -q --no-clone-bundle
```
