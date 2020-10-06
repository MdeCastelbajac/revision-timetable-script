# Retrospective Timetable Generator
A Python script using bash to generate and/or update retrospective revision timetables in *csv* format

### What is a retrospective timetable ?
A retrospective timetable is basically a reversed timetable where data is expressed in time-unit and sorted by subject instead of being the other way around. 
It is supposed to be filled retrospectively, which means the table gives you the information on *"what was done when (and how)"* instead of *"What to do next"*

This typically helps organizing per-topic following through time. In my case, this applies to exams' revisions.  
### How it works
- Regarding how you set-up your directory tree, the scripts reads the information it needs to build or update a *csv* file, a spreadsheet, and the rows in it.    
  The default one is :
  
  **Field (file) -> Subject (sheet) -> Course (row)**

- (Optional) You may want to keep track of an indicator (urgency, difficulty, confidence, etc.) per session :
  In this case, the base version comes with a 3-color set (RYG) which you can chose from, using the command line.
  
- Then it fills the first non-empty cell on the matching row with the current date and a bg-color, if specified (*see above*).
  and opens the up-to-date timetable.



