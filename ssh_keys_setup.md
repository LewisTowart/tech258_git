# SSH

### How to create and link repos with a SSH key

First we need to navigate to our ssh folder where our keys are stored
![locate.png](Markdown_Images%2Flocate.png)

We are then going to generate out two keys both public and private
![generate_key.png](Markdown_Images%2Fgenerate_key.png)

You can see here I am checking to make sure they have been created
![created_visual.png](Markdown_Images%2Fcreated_visual.png)

For the next step we need to copy out newly created public key
![show_key.png](Markdown_Images%2Fshow_key.png)

Now we need to add out newly created public key to our settings page on the repo we are targeting. Make sure to click the box for allow write access.
![online_repo_ssh.png](Markdown_Images%2Fonline_repo_ssh.png)

For us to access our repo and continue to add/commit changes we now need the SSH key. To use the key we need to add it to the keyring of sort in the repo location.
![keyring_add.png](Markdown_Images%2Fkeyring_add.png)

It's important to also activate github as a known host for our key
![github.png](Markdown_Images%2Fgithub.png)

