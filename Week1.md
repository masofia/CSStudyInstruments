Week 1 Progress Report

- Setup crash simulator environment. 

- Stuck for long time because Docker installation was not working. 

- Got manual installation working.

- Ran simulator with 'ls' and 'cp'. 
  With both applications, when running rreplay on the test, there was no output, the simulator just hung.
  
- When running these again after class, was able to get output. 
  I must have been following the instructions incorrectly before, not aligning events properly maybe or choosing lines that are part of the loading of the lib. 
  
- Tried modifying file types for 'ls', 'cp', 'tail'. Saw problems with the 'openat' system call since this was not supported.
