Week 4 Progress Report

- Tested fix for previously unhandled system call `fchmodat` and `clock_gettime`.
  
- Tested fix for system call `clock_gettime`. Still seeing errors related to `clock_gettime` when using the libs `fs.copysync`, `fs.writeJsonSync`, `fs.moveSync`
  Tracked in issue: [Issue 67](https://github.com/pkmoore/rrapper/issues/67)
  Issue was fixed during class - no longer seeing this issue
  
- Tested multiple functions in NodeJS library `loadash`  

- Ran into error `"bad interpreter: too many levels of symbolic links"`. Reinstalling python did not fix this. Created new VM and tried to install everything from scratch but encountered errors setting up rr. 
    - Preston was able to fix issue with symbolic links during class.
    - After this environment issue was fixed, I started seeing a new error when running the tests for the NodeJS libraries - created issue - https://github.com/pkmoore/rrapper/issues/82
