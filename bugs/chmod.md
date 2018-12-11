## Meta
* Project: chmod
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug identified as not a bug
* Brief description:
The chmod command does not error when the filetype is changed in crash simulator.


## Updates

### Week 3

**Current Stage: Bug Identified**

Possible bug discovered when changing file types in an fstat call with rreplay. When file type is changed and rreplay is run, there is no crash.

### Week 5

**Current Stage: Bug identified as not a bug**

It is expected that mutating the file type here will not crash since chmod just changes permissions of files. 
