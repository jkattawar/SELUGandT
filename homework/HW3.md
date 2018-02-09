# Homework Three

Fill out this worksheet (it can be opened in a plain text editor, like TextEdit [Mac] or TextWrangler [Mac] or Notepad [Windows]. Commit and push it to your copy of the course repo. I will pull your copies Friday at 5, and try to have comments for you by next class period, when we will discuss them. 

Feel free to work in groups, and discuss the assignments as needed. However, I do expect you to turn in your own copy, with answers in your own words. Feel free to try the commands in the answers - you don't have to do this from memory.

1. Matching: On LONI, when I log in, I am located in my _B_. I should store my data in the _A_ system, which has a 60 day storage limit.
 I should run computations in the _A_, and not in the _B_.

	a. /work/  
	b. user home

2. If I wanted to view the files in my home directory, but I am located in my work directory, I would use:  
	a. ls  
	b. ls -F  
	c. ls ~/ 
The answer is C (ls ~/)
	
3. In your own words, what does the correct command in question two do? 

The command ls ~/ lists the files in your home directory

4. In what order do we use the following commands: git push, git add, git commit? In your own words, what does this series of commands do? 

git add, git commit, git push- this series of commands pushes a file to a repository of your choice. In our case the GandT Lab repository on github.

5. This series of commands will not work. Can you spot the issue? Tell me what goes wrong here, and why.

```
mkdir my_project
cd my_project
mkdir data output scripts
nano readme
git add readme
git commit -m "adding my readme file!"
git push
```
git commit -m should be git commit -a. -m adds the commit message directly. We want to automatically stage the existing files with -a.
