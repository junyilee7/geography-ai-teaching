# 如何在 Mac 把檔案上傳到 GitHub（零經驗版）

你的 repo：https://github.com/junyilee7/geography-ai-teaching

推薦用 **GitHub Desktop**——一個免費的圖形介面 App，全程點按鈕，不用打任何指令。學會後以後每次更新都只要 3 個動作。

---

## 一、安裝 GitHub Desktop（只做一次）

1. 打開瀏覽器，到 https://desktop.github.com
2. 點「Download for macOS」，下載後安裝（拖進「應用程式」資料夾）
3. 打開 GitHub Desktop，點「Sign in to GitHub.com」，用你的 GitHub 帳號（junyilee7）登入
4. 登入後它會問是否設定 Git 名稱與 email，照預設按下一步即可

---

## 二、把你的 repo「複製」到電腦上（只做一次）

GitHub 上的 repo 是「雲端版」，你要先把它下載成「本機版」才能編輯。

1. GitHub Desktop 上方選單：`File` → `Clone repository`
2. 在清單裡找到 `junyilee7/geography-ai-teaching`，點它
3. 「Local path」是它會存到電腦的哪裡——記住這個路徑（例如 `/Users/leejunyi/Documents/GitHub/geography-ai-teaching`）
4. 點「Clone」

完成後，你的電腦上就有一個 `geography-ai-teaching` 資料夾，裡面是 repo 的內容。

---

## 三、替換成新檔案

1. 打開 Finder，到剛剛 clone 下來的 `geography-ai-teaching` 資料夾
2. **把裡面看得到的檔案和資料夾全部刪掉**
   （`notebooks` 資料夾、`README.md`、`LICENSE` 等等都刪掉。
   注意：有一個隱藏的 `.git` 資料夾你看不到，不用管它，不要去動它。）
3. 打開另一個 Finder 視窗，到我準備好的新版資料夾：
   `/Users/leejunyi/Disc/personal/教職/台南大學2026/geography-ai-teaching/`
4. 把新版資料夾裡的**所有檔案與資料夾**（README.md、SETUP.md、LICENSE、requirements.txt、`.gitignore`、`_build_notebooks.py`、`notebooks/`、`assets/`）全部複製，貼到第 1 步那個 clone 下來的資料夾裡
   - 小提醒：`.gitignore` 是隱藏檔。在 Finder 按 `Cmd + Shift + .` 可以顯示隱藏檔，確保它有被複製到。

---

## 四、上傳（每次更新都做這 3 步）

1. 回到 GitHub Desktop，它會自動偵測到你改了哪些檔案，左側會列出一串變更
2. 左下角有兩個欄位：
   - 上面那格（Summary）打一句話描述這次改了什麼，例如：`Rewrite as a general geography-AI teaching resource`
   - 點藍色按鈕「**Commit to main**」
3. 接著上方會出現「**Push origin**」按鈕，點它

完成！打開 https://github.com/junyilee7/geography-ai-teaching 重新整理，就會看到新內容。

---

## 五、補一個 repo 描述（建議）

1. 到 https://github.com/junyilee7/geography-ai-teaching
2. 右上方「About」旁邊有個齒輪圖示，點它
3. 「Description」欄填：
   `Reproducible Jupyter notebooks for bringing AI and computational methods into geography teaching.`
4. 點「Save changes」

這樣 repo 首頁原本的「No description」就會消失。

---

## 以後要再更新時

只要重複「**三、替換檔案**」和「**四、上傳**」即可。GitHub Desktop 會記住一切，不用再 clone。

---

## 如果懶得裝 App：純網頁的做法（適合一次性）

1. 到 https://github.com/junyilee7/geography-ai-teaching
2. 逐一點開舊檔案 → 右上垃圾桶圖示刪除 → 底部「Commit changes」
3. 全部刪完後，點「Add file」→「Upload files」
4. 把新版資料夾的檔案拖進去（可以整個資料夾拖，會保留結構）
5. 底部「Commit changes」

網頁版每次只能處理少量檔案、較繁瑣，所以還是建議用 GitHub Desktop。
