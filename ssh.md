# SSH

## What permissions do I need for SSH login using keys to work?

On the server, make sure to do:

```
chmod go-w /home/$USER
chmod 700 /home/$USER/.ssh
chmod 644 /home/$USER/.ssh/authorized_keys
```

Source:

https://superuser.com/questions/215504/permissions-on-private-key-in-ssh-folder
