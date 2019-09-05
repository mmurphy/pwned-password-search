# pwned-password-search

A list of hashed real world passwords that have involved in data breaches is available at (Troy Hunt's Have I Been Pwned: Pwned Passwords site)[https://haveibeenpwned.com/Passwords]
It's possible to hash a password, and then search the file to check if it has been previously compromised.  I had used `grep` to search the file, which works, but can take 10 or 15 minutes to search.

I wanted to write a tool which would work faster, by doing a binary search of the sorted file.  A slight complication is that the lines in the file are not the same length.

Hence the reason for writing this tool.

If you are looking for an existing tool, then `look` might be a better one for you, since it's been around for quite a while.

I'm using this as an exercise in file handling using golang

