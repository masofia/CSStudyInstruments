Week 5 Progress Report

- Reviewed a few of the past tested apps/libs. 
  - Updated potential bugs identified as not bugs: [chmod](https://github.com/masofia/CSStudyInstruments/blob/master/bugs/chmod.md) and [pwd](https://github.com/masofia/CSStudyInstruments/blob/master/bugs/pwd.md)
  - Created [issue 84](https://github.com/pkmoore/rrapper/issues/84)
  - `fs-extra.moveSync` -> possible bug identified when no error with file type mutator -> determined it was expected behavior
  - `fs-extra.copySync` -> possible bug identified when no error with file type mutator -> determined it was expected behavior 

- Continued testing NodeJS libs lodash, fs, csv-parser: `lodash.sortBy`, `fs.createReadStream`, `csv-parser`

- Created [issue 89](https://github.com/pkmoore/rrapper/issues/89)

- Looking at other NodeJS libs - `fs.copy` handles character and block devices properly: https://github.com/jprichardson/node-fs-extra/issues/193 
