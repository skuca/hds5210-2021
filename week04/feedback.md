Part 1:  5/5

Part 2:  4/5

20.4 - Using Pandas as you did certainly works, but it's a lot more code than necessary.  The approach I would recommend on this is to start by looping over the list of patients.  For each patient, take the diagnosis and use it to get the associated length of stay from the `avg_los` dictionary.  Then you can compare that to the patient's lenght of stay.  -1

So, something like this:

```
for patient in patients:
  name = patient[0]
  diagnosis = patient[1]
  length_of_stay = patient[2]
  average_days = avg_logs[diagnosis]
  
  if length_of_stay == average_length_of stay:
    conclusions = "just right"
  ...
```
