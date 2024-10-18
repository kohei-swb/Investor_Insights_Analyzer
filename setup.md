## Virtual environment
```bash
source env_name/bin/activate
```

## setup
cd your_project # Navigate to your project folder
python -m venv venv # Create virtual environment
source venv/bin/activate # Activate virtual environment
pip install -r requirements.txt # Install your packages
deactivate # Deactivate venv
git init # Initialize repo
echo 'venv' > .gitignore # Add venv to .gitignore
git add .
git commit -m 'initial commit'
git push


## branch
git checkout -b new-branch-name 
git add [ファイル名] 　　　　　　　        //追加
git commit -a -m "任意のコメント"  　     //コミット
git push origin ブランチ名                               //リモートを更新（リモートリポジトリにもブランチが作成される）

git push origin kohei-branch
git reset --soft HEAD~1  //delete the last commit and leave the changes

## postgresql with elastic search
brew install postgresql
brew services start postgresql
psql -h localhost -p 5432 -U kohei -d postgres
