## Homework #1: Terminal
All commands are executed on the MacBook

1) See "Where am I?" in my computer: `pwd`

2) Create a new folder: `mkdir folder_name`

3) Go to the folder: `cd folder_name`

4) Create 3 folders: `mkdir folder_name1 folder_name2 folder_name3`

5) Enter any folder you just created: `cd folder_name1`

6) Create 5 files (3 txt, 2 json): `touch file1.txt file2.txt file3.txt file4.json file5.json`

7) Create 3 new folders: `mkdir folder1 folder2 folder3`

8) Show list of folder contents: `ls -la (list of files + hidden files will be visible)`
9) Open any txt file: `vim file1.txt`

10) Write any text in the file:
```
On the keyboard, press i (insert)
Enter any text
Press esc :wq (save text and exit) + enter
```
12) Navigate up one directory: `cd ..`

13) Move any 2 files to any other folder:
```
mv file1.txt file4.json destination/
or
mv {file1.txt,file4.json} destination
```
14) Copy any 2 files you created to any other folder:
```
cp file1.txt file4.json destination/
or
cp {file1.txt,file4.json} destination
```
15) Find a file by name: `find ./ -name file1.txt`

16) View content in real-time: `tail -F file1.txt`

17) Display the first few lines from a text file:
```
head -n2 file1.txt
(the nunber indacates the number of lines that we want to view)
```
18) Display the last few lines from a text file:
```
tail -n5 file1.txt
(the number indacates the number of lines that we want to view)
```
19) View the contents of a long file: `less file1.txt`

20) Display date and time: `date`

---

##### Task 1* Send an HTTP request to the server: http://162.55.220.72:5005/terminal-hw-request:
```
curl 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000'
curl -v 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000' - (make the operation more talkative)
```

##### Task 2** Write a script that will automatically complete steps: 3, 4, 5, 6, 7, 8, 13
```
touch script.sh
chmod -x script.sh
vim script.sh
(on the keyboard, press i (insert))
cd folder_name
mkdir folder_name1 folder_name2 folder_name3
cd folder_name1
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir folder1 folder2 folder3
ls -la
mv file1.txt file4.json folder3/
(on the keyboard, press esc :wq (Save text and exit) + enter))
./filename.sh
```
