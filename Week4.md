Week 4 Progress Report

- Tested fix for previously unhandled system call `fchmodat` and `clock_gettime`.
  
- Still seeing errors related to `clock_gettime` when using the libs `fs.copysync`, `fs.writeJsonSync`, `fs.moveSync`
  Tracked in issue: [Issue 67](https://github.com/pkmoore/rrapper/issues/67)
  
- Tested NodeJS libraries:
  
