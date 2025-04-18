#Початкове налаштування
echo "# Завдання 1: Git & GitHub Основи" >> > Task1/README.md \n
git init \n
git add README.md \n 
git commit -m "Add Task1/README.md" \n
git branch -M main \n
git remote add origin https://github.com/kushch-a/test.git \n
git push -u origin main \n

#Гілки та пуш
git checkout -b dev \n
echo "Test test test file" > test.txt \n
git add test.txt \n 
git commit -m "Add test.txt in dev" \n 
git push origin dev \n

git checkout -b kushch-a-new_feature \n
echo "# New Feature by kushch-a" > README.md \n
git add README.md \n 
git commit -m "Add README.md in kushch-a-new_feature" \n
git push origin kushch-a-new_feature\n 

git status \n

# Команди Git
echo ".*" > .gitignore\n
git add .gitignore\n
git commit -m "Add .gitignore to ignore dotfiles" \n
git push origin kushch-a-new_feature \n 

\n
#Pull Requests та злиття
- Merge вручну kushch-a-new_feature → dev\n
git checkout dev\n
git pull origin dev\n
- Merge вручну  dev → main\n
git checkout main\n
git pull origin main\n
git checkout kushch-a-new_feature\n
nano README.md\n
git add README.md\n
git commit -m "Edit README.md temporarily"\n\n

#Скасування та лог
git reset --hard HEAD~1\n
git log > log.txt\n\n

git checkout main\n
git pull origin maingit add log.txt\n
git commit -m "Add git log to log.txt from kushch-a-new_feature"\n
git push origin main\n\n

#Очищення
git branch -d kushch-a-new_feature\n
git push origin --delete kushch-a-new_feature\n\n


git checkout dev\n
nano git_commands.md \n
git add git_commands.md\n
git commit -m "Add git_commands.md with used Git commands"\n
git push origin dev\n
