# SSH

## What permissions do I need for SSH login using keys to work?

On the server, make sure to do:

```
chmod go-w /home/$USER
chmod 700 /home/$USER/.ssh
chmod 644 /home/$USER/.ssh/authorized_keys
cat id_rsa.pub > authorized_keys
```

Source:

https://superuser.com/questions/215504/permissions-on-private-key-in-ssh-folder

## Generate new SSH key

```
ssh-keygen -t rsa -b 4096 -C "you@email.com"
```

Save the file and type in secure passphrase.

Add to `~/.ssh/config`:

```
Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa
```

Add private key to ssh-agent:

```
ssh-add -K ~/.ssh/id_rsa
```

Source: https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
