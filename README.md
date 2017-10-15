# google-spreadsheet-scheduler
These are a collection of scripts that perform functions to auto schedule students enrolled in a public speaking course into various parts on the sheet.  The schedule is contained on one sheet (CLMSchedule) while the students are contained on another (Students) sheet.  The functions work by auto rotating the students into the parts on a weekly basis.  It does this by getting the row number and value of the last student assigned in the specific column for that assignment and recording these to other cells located elsewhere and assigning variables to these ranges.  It then loops through the student names on the student sheet and compares if the value is equal to the value of the last student assigned for that column. If so, it then gets all the students in the student list after this name, copies them and pastes them to the schedule, starting at the very next empty row.  There are other functions that limit how many times the function loops and functions that will start the loop again at the first row in the list of students once it gets to the last row of students in the list.  
