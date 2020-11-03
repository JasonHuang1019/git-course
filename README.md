# git-course

![image](https://github.com/JasonHuang1019/git-course/blob/main/git-workflow.png)

Git 可以分為 Local（本地）和 Remote（遠端）兩個環境，由於 Git 屬於分散式的版本控制系統，所以開發者可以在離線 local 環境下開發，等到有網路時再將自己的程式推到 Remote 環境或 pull 下其他開發者程式碼進行整合。在 Local 中我們又分為 working directory（工作資料夾）、staging area（暫存區）和 repositories（檔案庫）。

當自己開發時會在工作資料夾工作，當要進入檔案庫之前會先將檔案加入暫存區，確認沒問題則 commit 到檔案庫中，最後 push 上去 remote 環境。在 Git 中若是有和其他開發者一起合作，則會需要處理不同 branch 之間 conflict 和 merge 的問題。

.gitignore：要忽略的檔案清單，這是用來告訴 Git，當在做版本控制記錄的時候，忽略這些檔案。
通常一些機密資料，如資料庫帳號密碼或是 server IP 位置等，記得要加入。也可以參考 github 上面的一些範本 在新增 repository 時選取對應的程式語言

README.md：repository 介紹和使用方式說明（例如：使用方法、參與專案方式等），使用 markdown 語法撰寫。另外通常有 CONTRIBUTING.md 額外說明如何參與貢獻。


 // 檔案尚未加入過追蹤時使用，即可恢復到檔案尚未加入暫存區
 $ git rm --cached hello.py


 // 若檔案已經在 repository 內，則使用以下指令
 // repository 與 stage 的檔案都會被還原到 HEAD，但 working directory 內的檔案不變
 $ git reset HARD





///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

資料來源:

#git原理概念教學
https://blog.techbridge.cc/2018/01/17/learning-programming-and-coding-with-python-git-and-github-tutorial/

#放入圖片教學(  ![image](picture or gif url)  )
https://medium.com/@stephyang/%E5%9C%A8github%E7%9A%84readme-md%E5%8A%A0%E5%85%A5%E5%9C%96%E7%89%87%E5%8F%8Agif%E7%9A%84%E6%96%B9%E6%B3%95-7282a4a63141
