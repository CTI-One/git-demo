# Exercise solution

After [this](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent),

## First person

```
git clone git@github.com:cti-one/git-demo.git
cd git-demo
echo "hello" >> hello-git.txt
git diff # optional
git add hello-git.txt
git status # optional
git commit -m 'hello git'
git status # optional
git push
```

## After someone else has made a change

```
git pull --rebase
```
