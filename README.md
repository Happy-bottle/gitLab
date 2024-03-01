# GIT

**1.檢查當前git版本**
`**$ git —version**`

**2.檢查設定檔**
`**$ git config —list**`

**3.設定user.name & user.email**
`**$ git config —global user.name “yourname”
$ git config —global user.email “youremail”**`

**4.文字編輯器**
`**:q**`(離開)
`**:w**`(儲存)
`**:wq**`(儲存並離開)

**5.路徑指令**
`**cd**` 切換目錄
`**cd..**` 回到上一層
`**ls -al**` 檢視全目錄

**6.在想要使用的資料夾生成 .git檔案**
`**$ git init**`

**7.檢視上次提交後是否有檔案更新**
`**$ git status**`

**8.新增檔案到暫存區or被git控管**

`**$ git add aaa.html**`(新增單一檔案使用)
`**$ git add *.html**`(新增同類型檔案使用)

`**$ git add --all**`(新增所有上次未變更檔案)

**9.提交到本地倉庫**
`**$ git commit -m "init commit"**`

`**$ git commit -m "update aaa.html"**` (如果有異動要重新add後再update上傳)
`**$ git commit -am "update aaa.html”**` (直接跳過add步驟update，只適用已被控管的檔案)

**10.檢視commit紀錄**
`**$ git log`
`$ git log —online`**(精簡模式)

**11.把異動紀錄些改到最近一次commit**
`**$ git commit —amend —no-edit**`

**12.修改最近一次的commit訊息**
`**$ git commit —amend -m ”new massage”**`

**13.還原異動(包括變更過的程式碼都會被刪除)**
`**$ git restore aaa.html**`

`**$ git restore --staged aaa.html**`(會保留異動狀態)

**14.取消控管**
`**$ git rm —cached ccc.html**`

**15.比較檔案差異**
`**$ git diff aaa.html**`
`**$ git diff --stage`** (檢視暫存區異動)

`**$ git log —online**` 叫出精簡紀錄後`**$ git diff 資訊碼 資訊碼**`(比較兩筆異動差異)

**16.輸出異動資訊**
`**$ git diff > page.diff**`

**17.檢視該檔案每一行程式碼的紀錄**

`**$ git blame aaa.html**`

**18.切換版本(退回工作區)**
`$ **git reset HEAD~~~~~`** (往前退5版) **⇒** `$ **git reset HEAD~5**`

`$ **git reset <commit>**`(也可直接輸入資訊碼退版)

**19.回到暫存區**

`$ **git reset —soft [版本指令]**` 

**20.回到上版本狀態**
`$ **git reset —hard[版本指令]`  (會異動程式)**

**21.檢視歷史commit紀錄**

`**$ git reflog**`

≤===================================>

**1.檢視分支**

`**$ git branch**`

**2.創建分支(會複製目前所在分支並創建到新的分支)**

**`$ git branch [分支名稱]`**

**3.移動分支**

**`$ git checkout [分支名稱]`**
**`$ git switch [分支名稱]`**

**4.分支做合併**

**`$ git merge [分支名稱]`**

**5.刪除分支**
**`$ git branch -d [分支名稱]`**

**6.創建並移動分支
`$  git checkout -b [分支名稱]**
**$ git switch -c[分支名稱]**`

**7.修改分支名
**git branch -M**`[新分支名稱]`**
**git branch -M**`[新分支名稱]`**


**重設<別名>url
https://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@github.com/Happy-bottle/gitLab.git
