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

## If you want to contribute in existing project, you can follow these steps:

1. Clone the project
    ```bash
    git clone <repo-ssh-url>
    ```

2. Create a new branch
    ```bash
    git checkout -b <branch-name>
    ```

3. Make changes

4. Add changes to staging
    ```bash
    git add .
    ```

5. Commit your changes
    ```bash
    git commit -m "<commit-message>"
    ```

6. If your local main is outdated, you can pull the changes from remote main

    * 6a. Checkout to your local main
        ```bash
        git checkout main
        ```
        
    * 6b. Pull the changes from remote main
        ```bash
        git pull origin main
        ```
    * 6c. Checkout to your branch
        ```bash
        git checkout <branch-name>
        ```
    * 6d. Merge main to your branch
        ```bash
        git merge main
        ```

7. Push your changes
    ```bash
    git push origin <branch-name>
    ```

8. Create a pull request

9. Wait for the review

10. If there are any changes requested, make the changes and push them to the same branch again (follow steps 3-7)

11. If there are no changes requested, your pull request will be merged


## Rename existing branch

1- Rename branch from github repository

2- Run these commands on your local repository 

```bash
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```
