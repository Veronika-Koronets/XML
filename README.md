# XML

## 1. Create an external repository called XML
Going to https://github.com/Veronika-Koronets?tab=repositories, then click "New", enter a name "XML", make it public and choose "Add a README file"

## 2. Clone repository to local PC
Im going to my new repository. Click Code-->Local-->HTTP and copy this link

```
kv@kvPC MINGW64 /d
$ git clone https://github.com/Veronika-Koronets/XML.git
Cloning into 'XML'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

## 3. Create new.xml file in the local repo

```
kv@kvPC MINGW64 /d
$ cd XML

kv@kvPC MINGW64 /d/XML (main)
$ vim new.xml
```

## 4. Add a file for tracking
Use git add -->git status 

```
kv@kvPC MINGW64 /d/XML (main)
$ git add .
```

## 5. Do commit file

```
kv@kvPC MINGW64 /d/XML (main)
$ git commit -m new.xml
[main e5ad429] new.xml
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml
```

 ## 6. Send the file to remote repository
 
```
kv@kvPC MINGW64 /d/XML (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 276 bytes | 69.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/XML.git
   b6b3023..e5ad429  main -> main
```

 ## 7. Edit the content of the “new.xml” file - write information about yourself (full name, age, number of pets, future desired salary). Everything is written in XML format.
```
kv@kvPC MINGW64 /d/XML (main)
$ cat > new.xml
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
kv@kvPC MINGW64 /d/XML (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   new.xml

no changes added to commit (use "git add" and/or "git commit -a")

kv@kvPC MINGW64 /d/XML (main)
$ git commit -am
error: switch `m' requires a value

kv@kvPC MINGW64 /d/XML (main)
$ git commit -am new.xml
warning: in the working copy of 'new.xml', LF will be replaced by CRLF the next time Git touches it
[main 60d270e] new.xml
 1 file changed, 9 insertions(+)

kv@kvPC MINGW64 /d/XML (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 425 bytes | 212.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/XML.git
   e5ad429..60d270e  main -> main
```

## 9. Create file preferences.xml
```
kv@kvPC MINGW64 /d/XML (main)
$ touch preferences.xml
```

## 10. In the preferences.xml file, add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in XML format.
```
kv@kvPC MINGW64 /d/XML (main)
$ vim preferences.xml

kv@kvPC MINGW64 /d/XML (main)
$ cat preferences.xml
<?xml version="1.0" encoding="UTF-8"?>
<preferences>
        <film>Legally_Blonde <film>
        <series> Blacklist <series>
        <food> pizza <food>
        <season> spring <season>
        <country> Norway <country>

</preferences>
```

 ## 11. Create a skills.xml file add information about the skills that will be studied in the course in XML format.
```
kv@kvPC MINGW64 /d/XML (main)
$ cat > skills.xml
<?xml version="1.0" encoding="UTF-8"?>
<skills>
        <skill1> Terminal <skill1>
        <skill2> GIT <skill2>
        <skill3> SQL <skill3>
        <skill4> Jmeter <skill4>
        <skill5> Postman <skill5>
        <skill6> Fiddler <skill6>



</skills>
```

## 12. Do one string commit
```
kv@kvPC MINGW64 /d/XML (main)
$ git add . && git commit -m "adding preferences.xml and skills.xml"
warning: in the working copy of 'preferences.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'skills.xml', LF will be replaced by CRLF the next time Git touches it
[main d2d4c56] adding preferences.xml and skills.xml
 2 files changed, 21 insertions(+)
 create mode 100644 preferences.xml
 create mode 100644 skills.xml
```

## 13. Send two files at once to the remote repository
```
kv@kvPC MINGW64 /d/XML (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 650 bytes | 216.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/XML.git
   60d270e..d2d4c56  main -> main
```

## 14. Create a bug_report.xml file on the web interface
## 15. Make Commit changes (save) changes on the web interface
## 16. Modify the bug_report.xml file on the web interface, add a bug report in XML format.
## 17. Make Commit changes (save) changes on the web interface.
## 18. Synchronize remote and local XML repository.
Use ``git pull`` command. ``git pull``= ``git fetch`` + ``git merge``
```
kv@kvPC MINGW64 /d/XML (main)
$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 2.02 KiB | 48.00 KiB/s, done.
From https://github.com/Veronika-Koronets/XML
   da29921..f465ca3  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 65 +++++++++++++++++++++++++++++++++++++++++++++++++++++++--------
 1 file changed, 57 insertions(+), 8 deletions(-)
```
