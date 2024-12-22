
1. Configure Git
If not already configured, set up your Git username and email:

git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

2. Initialize Git Repository
Navigate to your project directory and initialize Git:
git init

3. Link to Remote GitHub Repository
Add your GitHub repository as a remote:
git remote add origin git@github.com:YourUsername/ec2-exercise.git

5. Exclude Unnecessary Files
Create a .gitignore file to exclude files like .bash_history or .ssh:
echo ".bash_history" >> .gitignore
echo ".bash_logout" >> .gitignore
echo ".bash_profile" >> .gitignore
echo ".bashrc" >> .gitignore
echo ".ssh/" >> .gitignore
echo ".lesshst" >> .gitignore

Add .gitignore to your repository:
git add .gitignore
git commit -m "Added .gitignore to exclude unnecessary files"

5. Stage, Commit, and Push Files
Stage only the required files:
git add data.txt script.sh

Commit the changes:
git commit -m "Added metadata and setup script"

Push the code to the GitHub repository:
git push -u origin master
