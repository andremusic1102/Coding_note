# Git
### 隨時檢查目前 Git 的狀態
    git status


</br>
</br>
</br>
</br>


# 工作流程

* 建立新專案 </br>
cd 到對的位置
```
    mkdir 資料夾名
    touch 檔案名.py
    git init
```

* 已有repo</br> 先拉取远程代码，并合并：
```
    git pull
```
## |||||||||||||||||||||修改檔案||||||||||||||||||||||||

## **狀態 unstage**
A. 添加当前目录的(所有)文件到暂存区：
```
    git add 檔名
    或上傳全部檔案
    git add .
    **不要忘記 .**
```
## **狀態 stage / Staging Area**
B. 提交记录：
```
    git commit -m '记录内容说明'
```
前兩項可以合併成代替：
```
    git commit -am '记录内容说明'

    git log
    查看所有的commit紀錄
```
## **狀態 saved**


* 推送程式碼至Remote端 (Push/Pull ：
```
    git push 
    or
    git push origin master
```

* 在GitHub上創建一個和本地端名稱相同的資料夾，專案描述可寫可不寫、權限設為開放、README不用勾選
```
    git remote add origin URL
    git push -u origin master
```
## **狀態 已上repo**










</br>
</br>
</br>
</br>
</br>

# Clone a new repo

## 法一 in terminal
1. cd 到對的資料夾

2.    
```
    git clone URL   
```
URL 要用http 

## 法二 in vs code
1. 
```
    commend + shift + p
    git:clone 
```
paste URL

2. 選擇要存的本地位置git 
3. 打這次修改的描述
    commend + enter
4. 更新，按左下角 上傳下載

</br>
</br>
</br>
</br>
</br>

# git 其他

### 建立 .gitignore
在 push 之前，要加入 .gitignore ，
它會幫我們擋住一些 不必要push的檔案 ，像 node_modules 裡的所有套件，網路上全部都下載得到 所以也就沒必要推到我們的 repository


### 1. 看 Git 設定內容：
    git config --list
會看到 usr.name / usr.email

ps. How to exit a git status list in terminal?
typing 
```
    q 
```
should get you out
</br>
</br>
### 2. Tips:互動模式 
    git add -i
打完這次commit的描述
</br>
</br>
### 3. vim insert 模式
ps 如果在Vim迷路打

    :cq[uit]!


Normal 模式，又稱命令模式，在這個模式下，無法輸入文字，僅能進行複製、貼上、存檔或離開動作。

要開始輸入文字，需要先按下 i、a 或 o 這三個鍵其中一個進入 Insert 模式，便能開始打字。
其中，i 表示 insert，a 表示 append，而 o 則是表示會新增一行並開始輸入。
在 Insert 模式下，按下 ESC 鍵或是 Ctrl + [ 組合鍵，可退回至 Normal 模式。
在 Normal 模式下，按下 :w 會進行存檔，按下 :q 會關閉這個檔案（但若未存檔會提示先存檔再離開），而 :wq 則是存檔完成後直接關閉這個檔案。


</br>
</br>
</br>
</br>



# Git Branch
