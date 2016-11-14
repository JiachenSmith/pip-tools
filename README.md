[![Build status](https://secure.travis-ci.org/nvie/pip-tools.png?branch=future)](https://secure.travis-ci.org/nvie/pip-tools)

pip-tools = pip-compile + pip-sync + pip-review
===============================================

A set of two command line tools to help you keep your `pip`-based packages
fresh, even when you've pinned them.

[You _do_ pin them, right?][0]

![pip-tools overview for phase II](https://github.com/downloads/nvie/pip-tools/pip-tools-phase-II-overview.png)


Installation
============

To install, simply use [pipsi](https://github.com/mitsuhiko/pipsi):

```console
$ pipsi install pip-tools
```

Or if you specifically want the features available from the future branch:
```console
$ pip install git+https://github.com/nvie/pip-tools.git@future
```

Decide for yourself whether you want to install the tools system-wide, or
inside a virtual env.  Both are supported.


Testing
=======

To test under all (supported) Python versions:

```console
$ tox
```

The tests run quite slow, since they actually interact with PyPI, which
involves downloading packages, etc.  So please be patient.


[![Flattr this][2]][1]

[0]: http://nvie.com/posts/pin-your-packages/
[1]: https://flattr.com/thing/882478/Pin-Your-Packages
[2]: http://api.flattr.com/button/button-static-50x60.png
[3]: https://bitheap.org/cram/
