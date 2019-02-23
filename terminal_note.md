# Git

### 建立新專案
cd 到對的位置

    mkdir 資料夾名

    touch 檔案名.py

    git init


    git add 檔名
    或上傳全部檔案
    git add .

###### Staging Area
    git commit -m '這次的修改描述'

    git commit -e
    可以有比較詳細的描述（多行）

    git status
    查看狀態

    git log
    查看所有的commit紀錄



# 推送程式碼至Remote端 (Push/Pull)

##### 在GitHub上創建一個和本地端名稱相同的資料夾，專案描述可寫可不寫、權限設為開放、README不用勾選

git remote add origin URL


git push -u origin master

推上去這個branch
















### Clone a repo

###### 法一 in terminal
    git clone URL   
URL 要用http 

###### 法二 in vs code
1. 
commend + shift + p
    git:clone 
paste URL
2.
選擇要存的本地位置
3.
打這次修改的描述
commend + enter
4.
更新
按左下角 上傳下載


### Terminal 用法

















##### 看 Git 設定內容：
    git config --list
會看到 usr.name / usr.email

ps. How to exit a git status list in terminal?
typing 
    q 
should get you out

### 檢查目前 Git 的狀態
    git status


### stange / unstange
會有Untracked files 

狀態 unstage
    git add 檔名
狀態 stage
    git commit 
    但不要這樣打很麻煩
    git commit -m "這次修改的描述"
    快速提交
狀態 儲存好


###### 先拉取远程代码，并合并：
    git pull
###### 添加当前目录的所有文件到暂存区：
    git add .
###### 提交记录：
    git commit -m '记录内容说明'
###### 推送到远程：
    git push origin master

    git add .
    git commit -m '记录内容说明'
# 可以用下面代替：
    git commit -am '记录内容说明'



ps 如果在Vim迷路打
    :cq[uit]!


##### vim insert 模式
Normal 模式，又稱命令模式，在這個模式下，無法輸入文字，僅能進行複製、貼上、存檔或離開動作。


要開始輸入文字，需要先按下 i、a 或 o 這三個鍵其中一個進入 Insert 模式，便能開始打字。
其中，i 表示 insert，a 表示 append，而 o 則是表示會新增一行並開始輸入。
在 Insert 模式下，按下 ESC 鍵或是 Ctrl + [ 組合鍵，可退回至 Normal 模式。
在 Normal 模式下，按下 :w 會進行存檔，按下 :q 會關閉這個檔案（但若未存檔會提示先存檔再離開），而 :wq 則是存檔完成後直接關閉這個檔案。


##### Tips: 一次加入全部的檔案
互動模式 
    git add -i
打完這次commit的描述



### Git Branch















