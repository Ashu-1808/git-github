# Git Working
<img width="1056" height="616" alt="image" src="https://github.com/user-attachments/assets/e38f19ef-b738-45c7-a7e1-d5ae78576358" />

# Authentication type https:
## Download github repository to local server 
````
git clone https://github.com/abhipraydhoble/OnCdec-B29.git
````

````
cd OnCdec-B29
````
## set up identity

````
git config --global user.name "abhipray"
````
````
git config --global user.email "abhipraydhoble@outlook.com"
````

## create files
````
touch index.html  style.css
````

## add files into staging area
````
git add index.html
````
````
git add style.css
````

## list staged files
````
git status
````
## commit files into local repository
````
git commit -m "this is my first commit"
````
## view commit history
````
git log
````
# How to genrate the token
## 1 Log in to GitHub
```
Go to 👉 https://github.com
 and sign in.
```
## 2 Open Developer Settings
```
Click your profile picture (top-right)

Select Settings

Scroll down → Developer settings

Click Personal access tokens

Choose Tokens (classic)
```
## 3 Generate New Token
```
Click Generate new token (classic)
(You may be asked to re-enter your GitHub password)
```
## 4 Fill Token Details
```
Note:
Example: git-token-laptop
```
```
Expiration:
Choose 30 days, 90 days, or No expiration (not recommended)

Scopes (Permissions) – select:

✅ repo → full control of repositories

✅ workflow (optional, for GitHub Actions)

✅ read:org (optional)

 For normal Git push/pull → repo is enough
```
## 5 Generate & Copy Token
```
Click Generate token

⚠️ IMPORTANT

Copy the token immediately

You will never see it again

Treat it like a password

🧑‍💻 Use Token with Git (HTTPS)
Clone Repository
git clone https://github.com/username/repository.git


When prompted:

Username → your GitHub username

Password → paste the token

Save Token (Optional – recommended)
git config --global credential.helper store


This prevents Git from asking again.

🔁 If Token Is Lost or Expired

Just:

Go back to Personal access tokens

Delete old token

Generate a new one
```







