#linux #piping
## Finding a previously used Command

If you know a keyword or part of command prompt entered you can search through previously used commands with the following command. 

`history 100 | grep [term]`
*Gets the last 100 commands used and pipes that output into grep which returns matches for the regular expression provided.*