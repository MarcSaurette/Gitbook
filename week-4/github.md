# Github

If you completed the previous lesson, your Markdown file should be ready. The next step is to **Push** \(or contribute\) the file to the original Repository \([/MedievalBook](https://github.com/MarcSaurette/medieval-book)\) you **Forked** in Week 2. 

There are two ways you can **Push** your content. Follow which ever tutorial matches your needs, either with [Github Desktop](github.md#push-via-github-desktop) or via the [Terminal](github.md#push-via-terminal).

### Push via Github Desktop

Check the documentation [here](https://help.github.com/desktop/guides/contributing-to-projects/) for help with the desktop app.

**Step 1:** Open the Github desktop app. Ensure that HIST4006 is selected as the "Current repository" in the top left corner. Underneath this should be a tab "Changes". It should be highlighted already and underneath it will be a list of changes you have made, such as the new markdown file you have created. If it is there, type in the reason you are updating your repository in the text box contained the words "Summary" \(something like "created new profile file"\). 

**Step 2**: Press the button "Commit to Master" at the bottom left corner. Then Press the "Push Origin" button in the top right corner. This "pushes" the files on your harddrive to the Github site.

**Step 3**. In your web browser, navigate to your online Github \(something like [https://github.com](https://github.com)/\[Your Username\]/HIST4006\) and create a pull request \(following the same instructions as you did in week 2\), so that you can sync your new file back to the shared repository.

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

