# Connecting VS Code to GitHub Repository

Follow these steps to connect your files from **VS Code** to **GitHub**.

## Step 1: Initialize Git in VS Code
1. Open **VS Code** and navigate to your project folder.
2. Open the terminal (`Ctrl + ~` on Windows/Linux or `Cmd + ~` on Mac).
3. Run the following command to initialize Git:
   ```sh
   git init
   ```

## Step 2: Connect to GitHub Repository
1. Create a new repository on **GitHub**.
2. Copy the repository **URL** (HTTPS or SSH).
3. In the VS Code terminal, run:
   ```sh
   git remote add origin <your-repo-url>
   ```
   Example:
   ```sh
   git remote add origin https://github.com/your-username/your-repo.git
   ```

## Step 3: Add and Commit Files
1. Track all files:
   ```sh
   git add .
   ```
2. Commit the changes:
   ```sh
   git commit -m "Initial commit"
   ```

## Step 4: Push to GitHub
1. If your GitHub repository is empty, set the default branch name:
   ```sh
   git branch -M main
   ```
2. Push your code to GitHub:
   ```sh
   git push -u origin main
   ```

## Step 5: Verify on GitHub
- Go to your GitHub repository online and refresh the page. Your files should now be there!

## Additional Notes
- Ensure **Git** is installed: [Download Git](https://git-scm.com/)
- To check Git version:
  ```sh
  git --version
  ```
- Configure Git (if not done already):
  ```sh
  git config --global user.name "Your Name"
  git config --global user.email "your-email@example.com"
  










# Creating a GitHub Repository Using Terminal in VS Code

## 1. Initialize a Git Repository Locally
Open your VS Code terminal and navigate to your project directory. Then run:

```sh
git init
```

This initializes a new Git repository in your folder.

## 2. Add and Commit Your Files
Stage all files:

```sh
git add .
```

Commit the files with a message:

```sh
git commit -m "Initial commit"
```

## 3. Create a GitHub Repository

### Option 1: Manually
- Go to [GitHub](https://github.com) and create a new repository.
- Copy the repository’s remote URL.

### Option 2: Using GitHub CLI (Recommended)
If you have GitHub CLI (`gh`) installed, run:

```sh
gh repo create <repo-name> --public --source=. --remote=origin
```

Replace `<repo-name>` with your desired repository name.

## 4. Link Your Local Repo to GitHub
If you created the repository manually, link it using:

```sh
git remote add origin <your-repo-URL>
```

## 5. Push Your Code to GitHub
Run:

```sh
git branch -M main
git push -u origin main
```


