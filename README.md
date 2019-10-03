# GCP and nodejs prepare script

this repo is intended to reproduce this issue [#1497](https://github.com/GoogleCloudPlatform/nodejs-docs-samples/issues/1497)

##### TLTR

The `prepare` task do not read the env variables

log-1.js and log-2.js should have the same output

###### Cloud Build logs

```
Step #1 - "builder": > gcptest@0.0.1 gcp-build /workspace
Step #1 - "builder": > node ./log-1.js
Step #1 - "builder":
Step #1 - "builder": File log-1.js says: undefined
```

###### AppEngine logs
```
File log-2.js says: Lorem ipsum
```
