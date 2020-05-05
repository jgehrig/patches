# Additional Steps Required

The latest version of hg-git (0.8.13) is broken and Python3 is not supported.

Since the latest release of Mercurial supports Python3, and Gentoo uses Python3 by default we must disable Python3 for mercurial to work with hg-git.

You must apply the patch, and also update the USE flags:
```
dev-vcs/mercurial PYTHON_TARGETS: -* python2_7 PYTHON_SINGLE_TARGET: -* python2_7
```
