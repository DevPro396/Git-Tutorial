# Git-Tutorial
git and github tutorial

## Git commands
git status -> for getting the status of the projects
git add . or git add <filename> -> to let git know of the new changes in the project
pit pull -> getting new changes from the repo
git commit -m "a meaningful message for commit" -> save's the changes locally
git push origin master -> push the changes to the github repo


# SSH Agent and Generating ssh key adding ssh key 

generate command for ssh key

ssh-keygen -t ed25519 -C "github@emailaccount.com"

save the file

> Enter a file in which to save the key (/home/YOU/.ssh/ALGORITHM): ~/.ssh/<new-ssh-key-name>
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]

Start the ssh-agent in the background.

eval "$(ssh-agent -s)"
> Agent pid 000000

Add your SSH private key to the ssh-agent.

ssh-add ~/.ssh/<key-name> !not one with .pub ext.
