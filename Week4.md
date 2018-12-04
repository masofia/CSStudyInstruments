Week 4 Progress Report

- Tested fix for previously unhandled system call `fchmodat` and `clock_gettime`.
  
- Tested fix for system call `clock_gettime`. Still seeing errors related to `clock_gettime` when using the libs `fs.copysync`, `fs.writeJsonSync`, `fs.moveSync`
  Tracked in issue: [Issue 67](https://github.com/pkmoore/rrapper/issues/67)
  
- Tested multiple functions NodeJS library `loadash`  

- Ran into error `"bad interpreter: too many levels of symbolic links"`. Reinstalling python did not fix this. Created new VM and installed everything from scratch. 
