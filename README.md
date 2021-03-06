#Git By SourceTree 教學

學習利用 SourceTree 來管理 Github 裡頭的 Repository

Github 網址 (https://github.com/)
圖解 Git(https://marklodato.github.io/visual-git-guide/index-zh-tw.html?no-svg)
SourceTree 官網(https://www.sourcetreeapp.com/)
SourceTree 教學(https://hackmd.io/s/Bymbf3y2)
Git 教學網站(https://backlog.com/git-tutorial/tw/intro/intro1_1.html)

---

##0 Github 帳號申請. SourceTree 安裝

##1 知識點. 觀念說明

repository 版本庫，分為本地端和 remote 端
workspace(Working Dictionary) 工作目錄，程式碼所在專案
stage(Index) 將改變放進暫存區域
clone 複製一份版本庫到本地端
checkout 從遠端複製一份分支到本地端
commit 提交改變
push 將提交上傳到 Remote repository
pull 將提交從遠端下載下來
branch 分支
merge 合併分支
reset 將改變從暫存區域移除
remove 刪除新增檔案
stash 將改變暫存放到抽屜

##2 知識點. Git.SourceTree 操作說明

1.如何將一個本地專案變成一個版本庫 Repository 2.如何建立一個 remote repository 3.如何從 remote repository 複製一份版本庫(clone from url) 4.如何將改變進行暫存(how to click?) 5.如何提交.上傳.下載改變(click buttons) 6.如何建立分支 7.如何取消改變或移除新檔案 8.如何建立.應用 stash 9.如何進行合併(大支吃小支)

##3 知識點. 如何規劃分支

master 正式服務器版本
dev 測試服務器版本
bugFix 錯誤修正版本
newFun 新功能開發版本

##4 知識點. 忽略檔案

.gitignore 檔案作用在於忽略不需要版本控管的檔案
https://github.com/github/gitignore/blob/master/Laravel.gitignore 

##5 知識點. 問題排除

1.為何無法變更別人的版本庫
因為 Github 的 public 只是開放下載權限，無法修改。必須讓作者邀請你作為 colaborate 才行，需從 Github 後台的 setting 設置

2.為何無法切換到其他的分支
請注意是否有未提交的改變，請先完成提交或執行 Stash 後在進行切換

3.為何進行 Push 時跳出錯誤，我已經是 colaborate 了壓?
請注意 remote repository 的同一個分支是否有新的版本，有的話必須要先 pull 下來處理合併後才能上傳。

4.當發生衝突之後該怎麼處理呢?
只要將發生衝突的內容檔案的======和<<<<<>>>>>刪除就算是解決衝突了。
