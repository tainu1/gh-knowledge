# GitHub Operation Manual

## Initial Setup

### Git Install

- Download git Client

  ```batch
    XXX
  ```

  ```batch
    git version
    git version x.xx.x
  ```

### Git Configuration

- Git config settings

  ```batch
    git config --global user.name "Taichi Ito"
    git config --global user.email taichiito@example.com
  ```

- GitHub SSH settings

  - Generate SSH Key

    ```batch
      cd ~/.ssh
      ssh-keygen -t rsa
      Generating public/private rsa key pair.
      Enter file in which to save the key (/Users/(username)/.ssh/id_rsa):
      Enter passphrase (empty for no passphrase):
      Enter same passphrase again:

      ❯ ls ~/.ssh
      authorized_keys  id_rsa  id_rsa.pub
    ```

  - Register SSH Key for GitHub

  - Connection Check

    ```batch
      $ ssh -T git@github.com
      Hi jinwatanabe! You've successfully authenticated, but GitHub does not provide shell access.
    ```

### Coding Workflow

#### On GUI

-

#### On CLI

- Clone Repository

  ```batch
    git clone https://github.com/XXX/XXX.git
  ```

- Create Branch

  - リモートリポジトリは GUI でブランチ作成
  - Create a new local branch based on one of the remote branches and move to that branch

    ```batch
      git checkout -b (新しいブランチ名) (元にするブランチ名)
    ```

- Check Branch

  ```batch
    git branch    //local branch only
    git branch -a //All branches(including remote branch)
  ```

- Switch Branch

  ```batch
    git checkout (branch name)
  ```

- Add staging area

  ```batch
    git add .           //all files
    git add (file name) //the specific file
  ```

- Restore staging change

  ```batch
    git restore --staged (file name)
  ```

- Commit to local Respository

  ```batch
    git commit -m "XXX"
  ```

- Sync local repository to remote repository

  ```batch
    git push
  ```

- fetch remote repository change

  ```batch
    git pull
  ```
