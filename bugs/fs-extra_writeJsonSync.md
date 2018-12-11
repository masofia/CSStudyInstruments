## Meta
* Project: fs-extra.writeJsonSync
* Project Bug Identifier: 
* Link to Bug on Project Bug Tracker: 
* Current Stage: Investigated and determined there is no bug 
* Brief description (This can change as you progress) :

The function `writeJsonSync` of the NodeJS library `fs-extra` does not error out when the file type of the file to write to is modified to a block device.


## Updates

### Week 3

**Current Stage: Testing**

Was seeing errors with the system call `clock_gettime`, so could not properly run trace. Created issue: https://github.com/pkmoore/rrapper/issues/67

### Week 4

**Current Stage: Bug identified and determined it is not a bug**

Crash Simulator was run on the following test app:
```
const fs = require('fs-extra');
fs.writeJsonSync('/home/sse/testfile.json', {name: 'test'});
```

When the file type of `/home/sse/testfile.json` is modified to a block device (S_IFBLK) on replay, the app does not crash. When testing with a block device file, the write fails. So it was determined that it is not a bug.
