## DailyTips
 Useful tips for daily life

# Solution of excel opening second/subsequent file(s) slowly
 - Open regedit and locate the following directories:
 
 HKEY_CLASSES_ROOT\Excel.CSV\shell\Open\ddeexe
 
 HKEY_CLASSES_ROOT\Excel.Sheet.12\shell\Open\ddeexec
 
 HKEY_CLASSES_ROOT\Excel.Sheet.8\shell\Open\ddeexe
 

 - Set default value to:
 [open("%1" /ou "%u")]

 This will disable Dynamic Data Exchange for opening Excel files from Explorer.
