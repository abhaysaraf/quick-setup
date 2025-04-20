> Please note that the following actions need to be performed only once. In future, the same setup maybe useful while you setup other projects.

# Step-1: Verify if ssh-keys are already set
```
ls ~/.ssh
```

# Step-2: Create a new set of ssh-keys
```
ssh-keygen -t ed25519 -C "your_email_id@example.com"
```
Note: You can pass any comment for -C argument.

> When prompted 'Generating public/private ed25519 key pair.
Enter file in which to save the key (/Users/youruser/.ssh/id_ed25519)'

Press enter/return key to generate keys at `~/.ssh`

> And for Enter passphrase for "/Users/lifesahihai/.ssh/id_ed25519" (empty for no passphrase)

You can set password or keep empty for the below prompt.

# Step-3: Verify if ssh-keys were generated successsfully
You should be seeing `id_ed25519` and `id_ed25519.pub` files at your `~/.ssh` directory.
```
ls ~/.ssh
```

# References
1. [Generate new SSH Keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
