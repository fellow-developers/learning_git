# Learning  Git and Github
This repository is created to learn how we can use git for our upcoming project.


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
