# LR6
Лабораторная работа №6

## Progress of work

### 1. Настройка клиента
![alt_text](img/config.png "git config")

### 2. Клонирование удаленного репозитория
![alt_text](img/clone.png "git lone")

### 3. Добавление файла через интерфейс гита
![alt_text](img/git_int.png "git interface")
### 4. История операция для каждой ветки
![alt_text](img/full-log.png "git log")
### 5. Последние изменения
    git diff
### 6. Слияние в ветку master, решение конфликтов
![alt_text](img/merge.png "git merge")
### 7. Сделать несколько комитов с изменениями
![alt_text](img/1commit.png "1 commits")
![alt_text](img/2commit.png "2 commits")
### 8. Хард откат комита
![alt_text](img/reset_hard.png "git reset")
### 9. Создать ветку для отчета
![alt_text](img/report_branch.png "git branch -b 'branch_name'")
## Command logs

- git config -l
- git clone git@github.com:reven-n1/LR6.git
- cd LR6/
- git pull

**/добавление файла через интерфейс гита/**

- git log
- git diff(git show commit~ commit)
- git checkout master
- git merge origin/branch1

**<details><summary>/решение конфликта/</summary>**

before

![alt_text](img/conflict.png "conflict")

after

![alt_text](img/nano_solved_conflict.png "conflict")</details>


- git add mergefile.txt 
- git commit -am "soleved merge conflict"

- git branch -d branch1

**/изменения в wtf.py - 1/**
- git add .
- git commit -am "1st change"

**/изменения в wtf.py - 2/**
- git add .
- git commit -am "2nd change"
- git reset --hard HEAD~2
- git checkout -b "report"

- mkdir img

## Форматированная история комитов

git log --pretty=format:"%h - %an, %ar : %s"

![alt_text](img/formated_log.png "formated git log")