# python_script named test_script.py
* generates two different reports from this internal ticketing system log file i.e., syslog.log. 
* This script will parse through each log entry in the syslog.log file by iterating over it and will create the following reports:
## Files generated :
1. **error_message.csv**:
* The ranking of errors generated by the system .
* A list of all the error messages logged and how many times each error was found, sorted by the most common error to the least common error. This report doesn't take into account the users involved.
2. **user_statistics.csv**:
* The user usage statistics for the service . 
* A list of all users that have used the system, including how many info messages and how many error messages they've generated. This report is sorted by username.
For each log entry will check if it matches the INFO or ERROR message formats using regular expressions for this. When getting a successful match will add one to the corresponding value in the per_user dictionary. If i get an ERROR message will add one to the corresponding entry in the error dictionary by using proper data structure.
