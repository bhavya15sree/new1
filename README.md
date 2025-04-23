# Clone a GitHub repository
git clone https://github.com/username/repo-name.git
cd repo-name

# Make a change
echo "Hello GitHub!" >> hello.txt

# Stage and commit the change
git add hello.txt
git commit -m "Add hello.txt"

# Push the change
git push origin main  # or 'master', depending on the default branch
