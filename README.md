README

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