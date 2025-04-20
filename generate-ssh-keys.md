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
Enter file in which to save the key (/Users/your-user/.ssh/id_ed25519)'

Press enter/return key to generate keys in your `~/.ssh` directory.

> And for Enter passphrase for "/Users/your-user/.ssh/id_ed25519" (empty for no passphrase)

When you created your SSH key, you were optionally asked to set a passphrase. This is like a password that adds an extra layer of security. It ensures that even if someone gets access to your private key file, they can’t use it unless they also know the passphrase. You can set a passphrase or just press enter/return key.

# Step-3: Verify if ssh-keys were generated successsfully
You should be seeing `id_ed25519` and `id_ed25519.pub` files in your `~/.ssh` directory.
```
ls ~/.ssh
```

# References
1. [Generate new SSH Keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. [Adding SSH Key to Github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).
