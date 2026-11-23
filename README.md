# For Windows

Download the official installer from git-scm.com/download/win


Run the .exe file and click through the setup wizard. The default options work well for most users.

# Open Command Prompt, PowerShell, or Git Bash and verify the installation:

git --version

# To push your local website to your `.github.io` repository and publish it via GitHub Pages, 

make sure your repository is named exactly `<your-username>.github.io` and your main HTML file is named `index.html` in the root folder.

1. **Navigate to your website folder:**
Open your terminal (Command Prompt, PowerShell, or Terminal) and change into the directory containing your website files:

```bash
cd path/to/your/website

```


2. **Initialize Git and stage your files:**
Turn the folder into a local Git repository and stage all files for commit:

```bash
git init
git add .

```


3. **Commit your files:**
Save a snapshot of your staged files:

```bash
git commit -m "Initial website upload"

```

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.


4. **Rename branch and connect to GitHub:** Replace <username.
with your actual GitHub username">
Set your default branch to `main` and link your local folder to the remote GitHub repository:

```bash
git branch -M main
git remote add origin https://github.com/<username>/<username>.github.io.git

git remote add origin https://github.com/dropthemove/dropthemove.github.io
```


5. **Push your code to GitHub:**
Upload your local commits to GitHub (you may be prompted to sign in via your browser or a Personal Access Token):

```bash
git push -u origin main

```


### Verify Your Live Site

1. Go to your repository on GitHub and click **Settings** > **Pages** (in the left sidebar).
2. Under **Build and deployment**, ensure **Source** is set to **Deploy from a branch**, and the branch is set to **`main`** / **`/ (root)`**.
3. Wait 1–3 minutes, then visit `https://<username>.github.io` to view your live website.

*(Note: For future updates to your site, you will only need to run `git add .`, `git commit -m "Update site"`, and `git push`.)*