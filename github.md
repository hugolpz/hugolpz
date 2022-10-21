### Create your github profile

1.  Open Github.com, create an account
2. Open https://github.com/new , create repository with the same name as your username
3. It creates https://github.com/YOURPSEUDO/YOURPSEUDO
4. Open it, click Add file > Create file.
5. Name it README.md, add the following content :
```
### Dear reader,

I am **{USERNAME}**. I'm an junior data scientist / analyst.

- 🔭 I’m currently working on {...}, a simple language learning tool.
- 🌱 I’m currently learning {...}.
- 👯 I’m looking to collaborate and exchange on {...}.
- 🤔 I’m looking for help to  {...}
- 💬 Ask me about {...}.
- 📫 How to reach me: {...} [@] mail.com
- ⚡ Fun fact: my favorite fruit is 🥭.
```
6. Fill the form as needed and publish (commit).

**Helpers:**

- Emojipedia: https://emojipedia.org
- Clean profile: https://github.com/athul
- Pretty profiles gallery: https://zzetao.github.io/awesome-github-profile/

### Clone locally, edit, publish online

1. Open https://github.com/
```
git clone https://github.com/USERNAME/REPOSITORYNAME   # adapt
cd ./REPOSITORYNAME
git status                           # Shows files (red) and recent monitored changes (green)
echo "- Love 🍣 too !" >> README.md  # Append new line, save changes to file.
git status                           # See changes
git add README.md                    # Add changes to git repositories
git status                           # See changes
git commit -m "Added food taste"     # Add to "commited" = bundle approved changes and comment.
git status                           # See changes
git push                             # Send to remote (cloud) = shared/published
```
You can now edit file in text editor to go faster. Then du the cycle git add, git commit -m "...", git push to publish.

### Git basics
```
git clone https://github.com/USERNAME/REPOSITORYNAME
cd ./REPOSITORYNAME
echo "This is my 🍣 !" > 🍣.txt # Create unmonitored file
git status                      # Shows files (red) and recent monitored changes (green)
git add ./🍣.txt                # Add to "stage" = start monitoring
git status                      # Shows recent monitored changes
git commit -am "added 🍣 file"  # Approve all staged (monitored) changes + comment
git status
git push                        # Push commited changes to cloud, shared with team
```

### See changes
``` 
mkdir GitTest && cd GitTest   # Create directory, move in.
git init                 # create git tracking repository
git status               # display changes: nothing yet
echo "🍙Rice" > 🍣.txt   # create in working area, not monitored
git status               # display changes: an untracked file !
git diff ./🍣.txt        # nothing since, not git-tracked
echo "🐟Salmon" >> 🍣.txt
git add ./🍣.txt         # add to "stage", start git-tracking
git diff ./🍣.txt        # see changes !
echo "🥦Broccoli" >> 🍣.txt
git diff ./🍣.txt        #
git status
```
### Clean and undo things
```
clear                   # clean terminal screen
git reset -- 🍣.txt     # back to working-untracked area. Opposite: `git add` 
git rm --cached 🍣.txt  # unstage, back to working directory.
git rm 🍣.txt           # unstage and remove from working directory
git restore 🍣.txt
rm -rf .git             # remove git tracking. Opposite: `git init`.
```

### Levels of sharing
```
echo "🥖🥩🥬🍅🥒" > 🍔.txt    # 1. Working directory = there but not git-tracked.
git add 🍔.txt                # 2. Stage = git-tracked.
git commit -m "create 🍔.txt" # 3. Commited = ready to share, grouped and commented
git push                      # 4. Pushed = cloud, github, gitlab
```

Create your github home page !

- Visit : https://github.com/demangejeremy/demangejeremy/blob/main/README.md
- Fork : rename with your username (important !)
- Edit content to your profile ! See also : https://emojipedia.org
