Week 3 Progress Report

- Encountered unhandled system call `clock_gettime` when testing `date` and `tar`. 
  Created issue: [Issue 67](https://github.com/pkmoore/rrapper/issues/67)
  
- Encountered unhandled system call `fstatat64` when testing `rm` and `tar`.

- Testing `chmod`:
    - Encountered error with `exit_group(` traceline. Found issue was already raised: [Issue 37](https://github.com/pkmoore/rrapper/issues/37). Fix mentioned in issue (removing the line from trace_snip.strace file) resolved it. 
    - Encountered syscall with no handler `fchmodat`. Created issue: [Issue 68](https://github.com/pkmoore/rrapper/issues/68)

- Tested NodeJS libraries.
    `express`: could not test app, could not reach the service 
    `fs-extra`: `readFile`, `readFileSync`, `copySync`, `readJsonSync`, `writeJsonSync`
    Errors encountered: 
      - unhandled system calls `sendfile64`, `clock_gettime` 
      - 2 types of `ReplayDeltaError`
      - `ValueError: need more than 0 values to unpack`
      - `TypeError: list indices must be integers, not str`
