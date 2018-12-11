## Meta
* Project: pwd
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug identified as not a bug
* Brief description:
The pwd command does not error when the filetype is changed from a IFCHR to something else in crash simulator.


## Updates

### Week 3

**Current Stage: Bug Identified**

Possible bug discovered when changing file types in an fstat call with rreplay. When file type is changed and rreplay is run, there is no crash.

### Week 5

**Current Stage: Bug identified as not a bug**

Looking at the fstat call where the filetype was changed, it is not possible to replace this file with a different file of a different type and try to reproduce it. This is not really a bug.
