# SSH

### How to create and link repos with a SSH key

First we need to navigate to our ssh folder where our keys are stored

![locate.png](Markdown_images%2Flocate.png)

We are then going to generate out two keys both public and private

![generate_key.png](Markdown_images%2Fgenerate_key.png)

You can see here I am checking to make sure they have been created

![created_visual.png](Markdown_images%2Fcreated_visual.png)

For the next step we need to copy out newly created public key
![show_key.png](Markdown_images%2Fshow_key.png)

Now we need to add out newly created public key to our settings page on the repo we are targeting. Make sure to click the box for allow write access.

![online_repo_ssh.png](Markdown_images%2Fonline_repo_ssh.png)

For us to access our repo and continue to add/commit changes we now need the SSH key. To use the key we need to add it to the keyring of sorts in the local repo location.

![keyring_add.png](Markdown_images%2Fkeyring_add.png)

It's important to test that the key has been set up correctly as well

![github.png](Markdown_images%2Fgithub.png)

We can now add, commit and push as usual because the github repo is aware we own the private key to access the server.

### How do the SSH keys work?

![SSH_Authentication.png](Markdown_images%2FSSH_Authentication.png)

When someone is trying to access information on a server such as a GitHub repo and they are going through SSH they will need the correct permissions. The public key assigned to the server or repo can be see by anyone and is considered to be the lock. It is
locking away the access to the server. That public key has a paired private key that can allow access to the server this should never be shared. Once the server is trying to be accessed it will challege the users rights. If the user has the correct private key they will be able to access the server in GitHub case this could be pushing new changes to the repo.

