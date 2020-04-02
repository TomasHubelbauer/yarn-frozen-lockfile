# Yarn Frozen Lockfile

If you get this despite running just `yarn` without passing in the said argument:

> Your lockfile needs to be updated, but yarn was run with `--frozen-lockfile`.

Make sure there is not a `.yarnrc` with `--install.frozen-lockfile true` in any of the
parent directories. I had one where I didn't expect it, so it didn't occur to me to
look and I've wasted a good amount of time on it. Just check it - just in case.
