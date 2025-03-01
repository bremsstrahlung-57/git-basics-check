# Git & GitHub Basics Challenge

Hey team! We're gonna do a quick Git workout to show off our skills before Hackhazards'25. Follow these steps and have fun with it.

---

## **Step 1: Clone the Repository**

1. **Clone the Repo:**

   ```bash
   git clone https://github.com/bremsstrahlung-57/git-basics-check.git
   ```

2. **Navigate into the Repo:**

   ```bash
   cd git-basics-check
   ```

## **Step 2: Add Your Name on the Main Branch**

1. **First, pull the latest changes to avoid conflicts:**

   ```bash
   git pull origin main
   ```
(Skip from here and go to Step 3)

2. **Open the names.txt file** in the main branch.

3. **Add your name** on a new line (e.g., "Alex").

4. **Commit and Push:**

   ```bash
   git add names.txt
   git commit -m "Add my name: [Your Name]"
   git push origin main
   ```

5. **Handling Merge Conflicts:**
   If others have pushed changes to the same file, you might see a merge conflict. Don't panic! Here's how to resolve it:

   ```bash
   git pull origin main
   # Now open the file and resolve conflicts
   # Look for <<<<<<< HEAD, =======, and >>>>>>> markers
   # Edit the file to keep all names including yours
   git add names.txt
   git commit -m "Resolve merge conflict and add my name"
   git push origin main
   ```

## **Step 3: Create a New Branch for Your README**

1. **Make sure you have the latest main branch:**

   ```bash
   git checkout main
   git pull origin main
   ```

2. **Create a Branch:**
   Name your branch using this format: `feature/readme-yourname`
   (Replace "yourname" with your actual name)
   
      In Git branch naming conventions, feature is not the branch name itself but rather a prefix or category indicating the purpose of the branch.
      In the original format `feature/readme-yourname`:

      * `feature/` is a prefix indicating this branch is for developing a new feature
      * `readme-yourname` is the specific name/description of what's being worked on

      This naming pattern is part of a convention called "GitFlow" where branches are categorized by their purpose:

      * `feature/` for new features
      * `bugfix`/ for bug fixes
      * `hotfix/` for urgent fixes
      * `release/` for release preparation

      So when someone creates a branch named `feature/readme-john`, they're indicating they're working on a feature related to a readme and their name is `John`.

   ```bash
   git checkout -b feature/readme-yourname
   ```
    
3. **Add Your README File:**
   Create a new file called `names.md` (or if you want, yourname.md) and add some info about yourself—fun facts, skills, anything cool.

## **Step 4: Commit Your README Changes**

1. **Stage Your File:**
    ```bash
    git add names.md #(should be the name for your file)
    ```
    (can also do `git add .` to add all files that is ready for being staged)

2. **Commit Your Changes:**
    ```bash
    git commit -m "Added my personal readme with details"
    ```

3. **Push Your Branch:**
    ```bash
    git push origin feature/readme-yourname
    ```
    
## **Step 5: Create a Pull Request (PR)**

1. **Go to GitHub:**
   Open your repo on GitHub in your browser.

2. **Initiate a PR:**
   You should see a prompt to create a pull request for your recently pushed branch. Click on it.

3. **Fill Out the PR Details:**
   - Title: Something like "Add my personal readme".
   - Description: Write a short blurb about what you added (e.g., "Added my readme file with some fun facts and details about my background").

4. **Submit the PR:**
   Once submitted, we or someone else on the team will review it and merge it into main.


## **Step 6: After Your PR is Merged**

1. **Switch back to the main branch:**
   ```bash
   git checkout main
   ```

2. **Pull the latest changes including your merged PR:**
   ```bash
   git pull origin main
   ```

3. **You can now delete your feature branch (optional):**
   ```bash
   git branch -d feature/readme-yourname
   ```

## **Useful Git Commands**

* **Check repository status:**
  ```bash
  git status
  ```

* **View commit history:**
  ```bash
  git log
  ```

* **View simplified commit history:**
  ```bash
  git log --oneline
  ```

* **Discard changes to a file:**
  ```bash
  git restore <filename>
  ```

## **Extra Tips**

* **Review Each Other's PRs:**
   Feel free to leave some friendly feedback on your teammates' pull requests.

* **Keep Your Commit Messages Clear:**
   Clear messages make everything smoother and help avoid confusion.

* **Use `git status` Often:**
   It's a helpful command to understand what's happening in your repository.

* **Don't Sweat the Small Stuff:**
   Mistakes happen—learn from them, laugh them off, and keep pushing forward.