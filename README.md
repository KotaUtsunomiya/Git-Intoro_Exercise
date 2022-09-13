# Git-Intoro_Exercise
- Git入門 演習問題提出用リポジトリ
- READMEはリポジトリと一緒に作成

## 実施ログ
```
coachtech % git init
coachtech % 
coachtech % ls
index.html	style.css
coachtech % git add -A
coachtech % git commit -m "first-commit"
coachtech % git remote add origin https://github.com/KotaUtsunomiya/Git-Intoro_Exercise.git
coachtech % git push -u origin main
To https://github.com/KotaUtsunomiya/Git-Intoro_Exercise.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/KotaUtsunomiya/Git-Intoro_Exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
coachtech %
coachtech % git status
On branch main
nothing to commit, working tree clean
coachtech % git fetch
coachtech % git merge origin/main
coachtech % git merge --allow-unrelated-histories origin/main
coachtech % git push origin main
（中略）
To https://github.com/KotaUtsunomiya/Git-Intoro_Exercise.git
   abca5f3..47d0c15  main -> main
coachtech % 
```
  
  
## cloneしてくるパターンでも実施(別のリポジトリで確認）
```
coachtech % ls
index.html	style.css
coachtech %
coachtech % git clone https://github.com/KotaUtsunomiya/Git-introduction-exercise.git
coachtech %
coachtech % ls 
Git-introduction-exercise	style.css
index.html
coachtech % mv style.css Git-introduction-exercise/
coachtech % mv index.html Git-introduction-exercise/
coachtech % cd Git-introduction-exercise 
Git-introduction-exercise % 
Git-introduction-exercise % ls -a
.		.git		index.html
..		README.md	style.css
Git-introduction-exercise % 
Git-introduction-exercise % git add -A
Git-introduction-exercise % git commit -m "first commit"
（中略）
To https://github.com/KotaUtsunomiya/Git-introduction-exercise.git
   999a235..022cfe0  main -> main
branch 'main' set up to track 'origin/main'.
Git-introduction-exercise % 
```
