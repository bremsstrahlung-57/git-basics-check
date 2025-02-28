# git-basics-check

# Git & GitHub Basics Challenge

Hey team! We're gonna do a quick Git workout to show off our skills before Hackhazards’25. Follow these steps and have fun with it.

---

## Step 1: Fork the Repository

1. **Fork on GitHub:**
   - Go to the main repo at:  
     `https://github.com/your_username/git-basics-check`
   - Click the **Fork** button in the top-right corner to create your own copy of the repo under your GitHub account.

---

## Step 2: Clone the Repository

1. **Clone the Repo:**

   ```bash
   git clone https://github.com/your_username/git-basics-check.git

2. **Navigate into the Repo:**

   ```bash
   cd git-basics-check

## **Step 3: Add Your Name on the Main Branch**
1. Open the names.txt file in the main branch.
2. Add your name on a new line (e.g., "Alex").
3. Commit and Push:

   ```bash
   git add names.txt
   git commit -m "Add my name: [Your Name]"
   git push origin main

## **Step 4: Create a New Branch for Your README**
1. Create a Branch:
    Name your branch using this format: `feature/readme-yourname`
    (Replace "yourname" with your actual name)

    ```bash
    git checkout -b feature/readme-yourname
    
2. Add Your README File:
  Create a new file called readme.md (or if you want, yourname.md) and add some info about yourself—fun facts, skills, anything cool.

## **Step 5: Commit Your README Changes**
1. Stage Your File:
    ```bash
    git add readme.md
2. Commit Your Changes:
    ```bash
    git commit -m "Add my personal readme with details"
3. Push Your Branch:
    ```bash
    git push origin feature/readme-yourname
    
## **Step 6: Create a Pull Request (PR)**
1. Go to GitHub:
   Open your repo on GitHub in your browser.

2. Initiate a PR:
   You should see a prompt to create a pull request for your recently pushed branch. Click on it.

3. Fill Out the PR Details:
   - Title: Something like "Add my personal readme".
   - Description: Write a short blurb about what you added (e.g., "Added my readme file with some fun facts and details about my background").
   - Submit the PR:
   Once submitted, we or someone else on the team will review it and merge it into main.


## Extra Tips
* Review Each Other’s PRs:
  Feel free to leave some friendly feedback on your teammates’ pull requests.

* Keep Your Commit Messages Clear:
  Clear messages make everything smoother and help avoid confusion.

* Don’t Sweat the Small Stuff:
  Mistakes happen—learn from them, laugh them off, and keep pushing forward
