# Github

If you completed the previous lesson, your Markdown file is ready. The next step is to **Push** \(or contribute\) the file to the Repository \([/MedievalBook](https://github.com/MarcSaurette/medieval-book)\) you **Forked** in Week 2. If you have not done so yet, click the link above and do so now. 

There are two ways you can **Push** your content. Follow which ever tutorial matches your needs, either with [Github Desktop](github.md#push-via-github-desktop) or via the [Terminal](github.md#push-via-terminal).

### Push via Github Desktop

Check the documentation [here](https://help.github.com/desktop/guides/contributing-to-projects/) for help with the desktop app.

### Push via Terminal

**Step 1:** Clone the repository to your computer by clicking **Clone** under the repository name. Copy the link provided \(this is the clone URL\).

**Step 2:** Open your terminal and change the directory \(cd\) to where you want your cloned repository to be made. I suggest somewhere like /Documents or your class folder if you've made one:

```text
~$ cd Documents
#or
cd Hist4006A
```

**Step 3:** Clone the directory using the git clone command and the clone URL you've just copied.

```text
git clone https://github.com/YOUR-USERNAME/MedievalBook
```

Press **Enter** to clone the repository.

**Step 4:** Move your Markdown file to the local directory you just created and go to that directory via your Terminal. 

```text
~$ cd MedievalBook
#check to see if your file was moved to this directory
~$ ls
#Your file lastname_firstname.md should be there before you continue.
```

**Step 5:** Git needs to know that it shouldn't be ignoring the new file:

```text
git add lastname_firstname.md
#Now we can commit it to our repository.
git commit -m "added lastname_firstname.md"
```

**Step 6:** Git needs to know which remote repository to sync the changes to:

```text
git remote add origin https://github.com/YOUR-USERNAME/MedievalBook.git
#Confirm this command with:
git remote -v
#the output should look like this:
#    origin https://github.com/YOUR-USERNAME/MedievalBook (fetch)
#    origin https://github.com/YOUR-USERNAME/MedievalBook (push)
```

Git is letting you know that you can both fetch and push content from this remote repository to your local one. 

**Step 7:** Push your content to Github! 

```text
git push
```

And you are done! Go online to your Github and check your repository for changes. If all was done correctly, your markdown file should now appear there.

