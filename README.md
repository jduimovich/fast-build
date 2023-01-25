# fast-build

This is a repo that has a Dockerfile and a random devfile copied from samples which uses that Dockerfile to build.

The Dockerfile is a stripped down file which basically packages up ubi8/minimal and adds a single command.
This should build very quickly and can be tested.

This can be used to test the minimal-build time for an e2e Stone Soup without a deployment. 
```
FROM registry.access.redhat.com/ubi8/ubi-minimal 
# simple command print unix name info
CMD [ "uname", "-a" ]
```
