See [[Release Process SoTA]]
There ought to be some GitLab Action that can automate the process

When running the `run` shell script for a given service, we have to switch users from `ubuntu` to `root` using `sudo su`. This effectively lets us run all subsequent commands a `root` which is dangerous (i.e. any file can be irrevocably deleted). We do this because if you try to run / restart a service now with a non-`root` user like `ubuntu`, you'll get an error when trying to create / write to the `logs` file (e.g. `logs/crud_service_logs` - a path specified in `logback-spring.xml` - because the logs file is in the `root` owner and group).

To fix: change the log file for each service (in every environment) to be owned by and in the group of `ubuntu` - then we won't have to run commands as `root` anymore
`chown -R ubuntu:ubuntu logs/crud_service.log` 
For now, instead we opted only to `sudo` for the restart command itself - can write some shortcuts in `.bashrc`, but I had an issue with this being run from the root directory