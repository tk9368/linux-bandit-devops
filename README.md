## Linux Practice (OverTheWire – Bandit)

- Practiced Linux using SSH-based wargames
- Solved Bandit levels 0–8
- Topics: permissions, hidden files, grep, find, pipes

## Proof
- Commands used 
level 0 
ls
cat readme


level 1
ls
cat ./-
./- tells shell that - is a file, not an option


level 2
ls
cat spaces\ in\ this\ filename
/ tells handle space


level 3
ls
ls -a
cd inhere
ls -a
cat .hidden
ls -a  show hidden files
cat show the data of file

level 4
cd inhere
file ./*
cat ./-file07
file show the type of file 


level 5
cd inhere
find . -size 1033c
cat ./maybehere07/.file2
find use for find the specific size of file


level 6
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
search base on owner , group , size


level 7
grep "millionth" data.txt
grep search text inside files


level 8
sort data.txt | uniq -u
sort groups duplicate lines
uniq -u prints only unique line




