# Git Cheatsheet

## Create new lightweight tag

`git tag v1.0`

## Push tags to remote servers

`git push --tags`

## Switch to another branch

`git checkout <name of branch>`

## Undo last commit

`git reset --soft HEAD~1`

## Download just the source code of a project

`curl -sL https://github.com/feihong/tutorial-boilerplate/archive/master.tar.gz | tar xz`

## Set email

`git config --global user.email "your_email@example.com"`

## Change remote repository URL

`git remote set-url origin git@github.com:USERNAME/OTHERREPOSITORY`

## Create new, empty repo, sync it to GitHub, and create the gh-pages branch:

```bash
USERNAME=feihong
REPONAME=repo-name
REPODESCRIPTION="repo description"

curl -u $USERNAME https://api.github.com/user/repos -d "{\"name\": \"$REPONAME\", \"description\": \"${REPODESCRIPTION}\"}"
git init
git remote add origin git@github.com:$USERNAME/$REPONAME.git
git remote -v
echo "$REPONAME" >> README.md
git add README.md
git commit -m "Initial commit"
git push -u origin master

cd /tmp
git clone git@github.com:$USERNAME/$REPONAME.git
cd $REPONAME
git checkout --orphan gh-pages
git rm -rf .
echo "Hello GitHub Pages!" > index.html
touch .nojekyll
git add .
git commit -a -m "Initial pages commit"
git push origin gh-pages
```

## Sources

- https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/
- https://help.github.com/articles/creating-project-pages-manually/
- http://stackoverflow.com/questions/2423777/is-it-possible-to-create-a-remote-repo-on-github-from-the-cli-without-ssh
