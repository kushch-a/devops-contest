# Початкове налаштування

echo "# Завдання 1: Git & GitHub Основи" > Task1/README.md  
git init  
git add README.md  
git commit -m "Add Task1/README.md"  
git branch -M main  
git remote add origin https://github.com/kushch-a/devops-contest.git  
git push -u origin main  

# Гілки та пуш

git checkout -b dev  
echo "Test test test file" > test.txt  
git add test.txt  
git commit -m "Add test.txt in dev"  
git push origin dev  

git checkout -b kushch-a-new_feature  
echo "# New Feature by kushch-a" > README.md  
git add README.md  
git commit -m "Add README.md in kushch-a-new_feature"  
git push origin kushch-a-new_feature  

git status  

# Команди Git

echo ".*" > .gitignore  
git add .gitignore  
git commit -m "Add .gitignore to ignore dotfiles"  
git push origin kushch-a-new_feature  

# Pull Requests та злиття

- Merge вручну kushch-a-new_feature → dev:

git checkout dev  
git pull origin dev  

- Merge вручну dev → main:

git checkout main  
git pull origin main  

git checkout kushch-a-new_feature  
nano README.md  
git add README.md  
git commit -m "Edit README.md temporarily"  

# Скасування та лог

git reset --hard HEAD~1  
git log > log.txt  

git checkout main  
git pull origin main  
git add log.txt  
git commit -m "Add git log to log.txt from kushch-a-new_feature on main branch"  
git push origin main  

# Очищення

git branch -d kushch-a-new_feature  
git push origin --delete kushch-a-new_feature  

git checkout dev  
nano git_commands.md  
git add git_commands.md  
git commit -m "Add git_commands.md with used Git commands"  
git push origin dev  
