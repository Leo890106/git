class address : https://www.youtube.com/watch?v=RGOj5yH7evk

git clone address  //open the repo on local
git add .  //track all the data in the dictiionary 
           //if you want to track specific file use 
git add filename

git branch  //check all branch and show what branch you select

git checkout branchname  //switch to another branch
git checkout -b branchname  //creat a new branch and switch to it

Why we need branch ?

    1.平行開發：分支允許開發人員同時進行多項工作而不互相干擾。例如，開發人員可以在不同的分支上同時開發新功能、修復錯誤或進行實驗性改動，確保各項工作彼此獨立。 
    2.維護穩定性：主分支（如 main 或 master）通常用於存放穩定且可發布的代碼。透過在其他分支上進行開發或測試，可以避免對主分支造成不穩定的影響，從而維護主分支的穩定性。 
    3.版本管理：分支使得團隊能夠同時維護多個版本的軟體。例如，當需要對已發布的版本進行補丁修復時，可以在專用的分支上進行，並在修復完成後合併回主分支。 
    4.實驗性開發：分支提供了一個安全的環境來嘗試新功能或技術，而不會影響主分支的穩定性。如果實驗性的代碼效果不佳，可以輕鬆地刪除該分支，而不會對主代碼庫造成影響。

push順序  git add  ->  git commit  -> git push

在pull之前先確認所在的分支與要拉的分支是否依樣  
pull順序  git branch -> git pull

在merge過後記得刪除分之
git branch -d branch_name

當多個branch做merge時 有可能發生合併衝突 git不知道該保留哪些東西而那些東西是多餘的此時需要人為介入去解絕
git merge branch-name

undo 撤銷commit回到某次的更改
git log查看更改的紀錄  ->  複製你要回到地版本的hash value  -> git reset hash_value

undo 撤銷commit回到某次的更改並刪除那之後的版本
git log查看更改的紀錄  ->  複製你要回到地版本的hash value  -> git reset --hard hash_value


Pull Request 的主要功能包括：

代碼審查：在合併代碼之前，團隊成員可以通過 Pull Request 平台對提交的修改進行審查，確保代碼質量和一致性。

討論與反饋：開發者可以在 Pull Request 中討論具體的代碼實現，提供反饋或建議，促進團隊間的溝通與協作。

持續整合：許多專案會在 Pull Request 上設置自動化測試，確保新代碼不會引入錯誤，維持專案的穩定性。

Pull Request 的一般流程：

分支開發：開發者從主分支創建一個新的分支，在該分支上進行功能開發或錯誤修復。

提交修改：完成開發後，將修改提交到自己的分支。

創建 Pull Request：在 GitHub 上，從該分支向主分支發起 Pull Request，描述所做的修改和目的。

代碼審查：團隊成員或專案維護者審查該 Pull Request，提出意見或建議。

合併代碼：經過審查和必要的修改後，專案維護者將 Pull Request 合併到主分支中。

這種流程確保了代碼的質量和專案的穩定性，同時促進了團隊協作和知識共享。


在 GitHub 上，是一種將他人專案的完整副本複製到您自己的帳號下的操作。這使您能夠在自己的儲存庫中獨立地進行修改，而不影響原始專案。

Fork 的主要作用包括：

獨立開發：透過 Fork，您可以在自己的儲存庫中自由地實驗、修改或添加新功能，而不會影響原始專案的穩定性。

貢獻回饋：如果您希望將自己的修改貢獻回原始專案，可以透過提交 Pull Request，請求專案維護者審核並合併您的更改。

學習與參考：Fork 也可用於學習目的，讓您深入了解他人專案的實現方式，並在此基礎上進行探索。

Fork 的一般流程：

Fork 專案：在 GitHub 上找到您感興趣的專案，點擊頁面右上角的「Fork」按鈕，將該專案複製到您的帳號下。

克隆到本地：在您的電腦上，使用 git clone 將 Fork 後的儲存庫複製到本地。

進行修改：在本地儲存庫中，創建新分支並進行所需的修改。

提交修改：將修改提交並推送到您在 GitHub 上的儲存庫。

提交 Pull Request：在 GitHub 上，從您的分支提交 Pull Request，請求原始專案的維護者審核並合併您的修改。

透過這種方式，Fork 促進了開源社群的協作與創新，讓更多人能夠參與到專案的開發與改進中。

