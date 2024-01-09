# git 
## Practice 1

Some git practice below.
- clone a repository to local;
- create a new branch;
- create a local file with a text;
- create a branch on Github;
- make a commit;
- merge branches;
- delete a branch

iliya.sanin@Iliyas-MBP git % git clone git@github.com:Iliya-Sanin/git.git
<p> iliya.sanin@Iliyas-MBP git % cd git
<p> iliya.sanin@Iliyas-MBP git % ls
<p> README.md

<p> iliya.sanin@Iliyas-MBP git % git branch
<p> * main
<p> iliya.sanin@Iliyas-MBP git % git branch my_project
<p> iliya.sanin@Iliyas-MBP git % git branch
<p> * main
<p>   my_project

iliya.sanin@Iliyas-MBP git % git checkout my_project
iliya.sanin@Iliyas-MBP git % echo Text for my file > my_file.txt 
iliya.sanin@Iliyas-MBP git % ls
README.md       my_file.txt

iliya.sanin@Iliyas-MBP git % git add .
iliya.sanin@Iliyas-MBP git % git status
iliya.sanin@Iliyas-MBP git % git commit -m "my first commit for this branch"
iliya.sanin@Iliyas-MBP git % git push --all
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 10 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'my_project' on GitHub by visiting:
remote:      https://github.com/Iliya-Sanin/git/pull/new/my_project
 * [new branch]      my_project -> my_project

iliya.sanin@Iliyas-MBP git % git branch
  main
* my_project

iliya.sanin@Iliyas-MBP git % git checkout main
iliya.sanin@Iliyas-MBP git % git merge my_project
iliya.sanin@Iliyas-MBP git % git branch
* main
  my_project
iliya.sanin@Iliyas-MBP git % git branch -d my_project
Deleted branch my_project 

