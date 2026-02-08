## 1 Open Terminal / Git Bash
```
Linux / macOS → Terminal

Windows → Git Bash (recommended)

## 2 Generate the Key Pair
ssh-keygen -t ed25519 -C "your_email@example.com"


👉 If your system doesn’t support ed25519, use:

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
## 3 Choose File Location
```
You’ll see:

Enter file in which to save the key (/home/user/.ssh/id_ed25519):


✔ Press Enter to accept default
(or give a custom name like github_key)
```
## 4 Set Passphrase (Optional but Recommended)
```
Enter a passphrase → extra security

Or press Enter to skip
```
## 5 Keys Generated 🎉
```
Your identification has been saved in id_ed25519
Your public key has been saved in id_ed25519.pub
```

## 📁 Location:
```
~/.ssh/

File	Purpose
id_ed25519	🔐 Private key (DO NOT share)
id_ed25519.pub	🔓 Public key (safe to share)
📋 View & Copy Public Key
cat ~/.ssh/id_ed25519.pub


Copy the full output starting with:

ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAA...
```

## 🔗 Add Public Key to GitHub
```
Steps:

Go to GitHub

Settings → SSH and GPG keys

Click New SSH key

Paste the public key

Save

✅ Test SSH Connection
ssh -T git@github.com
```
```
Expected output:

Hi username! You've successfully authenticated.
```
| 🧠 Common Mistakes to Avoid | Fix permissions if needed |
|-----------------------------|---------------------------|
| ❌ Sharing private key | chmod 700 ~/.ssh |
| ❌ Wrong file permissions | chmod 600 ~/.ssh/id_ed25519 |
| ❌ Copying .pub partially | chmod 644 ~/.ssh/id_ed25519.pub |




