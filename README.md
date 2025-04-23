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
import requests

# Replace with your personal access token
token = "your_github_token_here"
headers = {"Authorization": f"token {token}"}

# Get user repos
response = requests.get("https://api.github.com/user/repos", headers=headers)

# Print repo names
for repo in response.json():
    print(repo["name"])
