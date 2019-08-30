# Helio Blueprints

TBD.

## Currently available BPs

**Busybox**
Nothing more than a docker container at this point. 
Only standard env variables
Runtime: $LIMIT * $SLEEP_TIME + start/stop time
Executable: `docker run` with a few env variables

**Docker**
Config with image, env vars, registry settings.
Additionally standard env variables
Runtime: unknown beforehand, depends on image
Executable: `docker run` -> CMD/Entrypoint with env variables set and maybe ARGS

**Ep85**
IDF + EPW (weather) data as input (as a file)
config json with files, SHA1 hash of files, report url and end result upload URL
run_id (?) as exec name
Additionally standard env variables
Runtime: estimation, but unknown initially + start/stop time
Executable: `docker run` which starts our own wrapping script, with env variables

**Gitlab**
Config with endpoint, token, tags, and possibly more settings for that runner
Additionally standard env vars (though they are not really needed)
Runtime: forever (but wouldn't it make sense to somehow have an execution per pipeline/job in gitlab?)
Executable: `docker run` gitlab-runner with a few ARGS

**Infinitebox**
Not more than a docker container at this point.
Config with image, env vars
Additionally standard env variables
Runtime: 0? almost 0 I guess
Executable: `docker run`
