# Learning  Git and Github
THIS REPOSITORY IS CREATED TO LEARN HOW WE CAN USE GIT FOR OUR UPCOMING PROJECT.


# GitHub SSH Setup

- Step 1
```bash
git config --global user.name "FIRST_NAME LAST_NAME"
```

- Setp 2
```bash
git config --global user.email "MY_NAME@example.com"
```

- Step 3
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

- Step 4
```bash
eval "$(ssh-agent -s)"
```

- Step 5
```bash
ssh-add ~/.ssh/id_ed25519
```

- Step 6
```bash
cat ~/.ssh/id_ed25519.pub
```
- End

# Create a new repository on the command line

```bash
echo "# Demo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:satyam-seth-learnings/reactjs_experiments.git
git push -u origin main
```

# Push an existing repository from the command line

```bash
git remote add origin git@github.com:satyam-seth-learnings/reactjs_experiments.git
git branch -M main
git push -u origin main
```

# Contribute in this project

Clone the project

```bash
git clone git@github.com:fellow-developers/learning_git.git
```

Go to the project directory

```bash
cd learning_git
```

Open Project in VSCode
```bash
code .
```
