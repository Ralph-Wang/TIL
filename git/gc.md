# git gc

Git also have a mechanism so called gc to clean up garbages that generated during the working.
git gc treat the objects seriously, as it don't delete object which is referenced by not only
the local work tree, but also the indexes, remote-tracking branches and other possible user.

More detail about the gc, refer to the document: [git-gc](https://git-scm.com/docs/git-gc)
