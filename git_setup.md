1. git config --global user.name "Your GitHub Username"
2. git config --global user.email "your_email@example.com"
3. check if SSH keys already exits `ls -al ~/.ssh`
4. If not, then generate the keys 
    `ssh-keygen -t rsa -b 4096 -C "your_email@example.com" `
5. `cat ~/.ssh/id_rsa.pub ` will display your public key. 
- Once the key is displayed, copy its contents.
- Go to your GitHub account settings.
- Click on “SSH and GPG keys.”
- Click “New SSH Key” or “Add SSH Key.”
6. add this under `~/.gitconfig`
    [url "ssh://git@github.com/"]
        insteadOf = https://github.com/


