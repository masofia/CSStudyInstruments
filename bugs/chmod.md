## Meta
* Project: chmod
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Possible Bug Identified
* Brief description:
The chmod command does not error when the filetype is changed in crash simulator.


## Updates

### Week 3

**Current Stage: Bug Identified**

Possible bug discovered when changing file types in an fstat call with rreplay. When file type is changed and rreplay is run, there is no crash.