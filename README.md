# XML
## 1. Create an external repository called XML
Going to https://github.com/Veronika-Koronets?tab=repositories, then click "New", enter a name "XML", make it public and choose "Add a README file"

## 2. Clone repository to local PC
Im going to my new repository. Click Code-->Local-->HTTP and copy this link
```
kv@kvPC MINGW64 /d/github_lesson/xml
$ git clone https://github.com/Veronika-Koronets/XML.git
Cloning into 'XML'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 9 (delta 1), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (9/9), done.
Resolving deltas: 100% (1/1), done.
```

## 3. Create new.xml file in the local repo
```
kv@kvPC MINGW64 /d/github_lesson
$ cd XML

kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ touch new.xml

```
## 4. Add a file for tracking
Use git add -->git status 
```
kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git add new.xml

kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git status new.xml
On branch main
Your branch is up to date with 'origin/main'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.xml
``` 
## 5. Do commit file
```
kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git commit -m "new.xml"
[main c06ea28] new.xml
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml
 ```
 
 ## 6. Send the file to remote repository
```
kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 277 bytes | 138.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/XML.git
   38046f2..c06ea28  main -> main
 ```
 
 
 ## 7. Edit the content of the “new.xml” file - write information about yourself (full name, age, number of pets, future desired salary). Everything is written in XML format.
```
kv@kvPC MINGW64 /d/Json (main)
$ vim new.xml

kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ cat new.xml
<?xml version="1.0" encoding="UTF-8"?>
<info>

        <person_name>K. Veronika Gennadyevna <person_name>
        <person_age>22 <person_age>
        <number_of_pets> 1 <number_of_pets>
        <future_desired_salary> 1300 <future_desired_salary

</info>       
``` 

## 8. Send the changes to remote repository
```
kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   new.xml

no changes added to commit (use "git add" and/or "git commit -a")

kv@kvPC MINGW64 /d/github_lesson/XML (main)
$ git commit -am "add info"
warning: in the working copy of 'new.xml', LF will be replaced by CRLF the next time Git touches it
[main 9926dcc] add info
 1 file changed, 10 insertions(+)
 
 
```
 
 
 
 
 
 
 
