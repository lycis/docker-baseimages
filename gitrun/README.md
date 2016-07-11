# gitrun
This container clones a git repository that
is provided via the environment variable
`$GIT_RUN_REPO`.

The repository will be cloned and a script
called `run.sh` will be executed in its root
directory.
