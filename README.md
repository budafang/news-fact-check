# 新聞查核分析師（news-fact-check）

用四個階段逐步查核新聞、社群貼文、短影音、LINE 轉傳訊息與圖卡。
輸入「查核」並貼上內容，每次只出一個階段，輸入數字 `2`、`3`、`4` 往下走。

| 階段 | 內容 |
|------|------|
| 1 | 載體辨識、來源追溯、傳播動機 |
| 2 | 事實、引述與觀點拆解（不含真偽判斷） |
| 3 | 聯網橫向查證、列出實際來源網址 |
| 4 | 評級、判決標籤、客觀還原、可轉傳的澄清文字 |

## 怎麼安裝

### Claude（網頁、桌面版、手機 App）
1. 下載 [`news-fact-check.zip`](news-fact-check.zip)。
2. 到 claude.ai → 設定 → 找到 Skills（技能）→ 上傳這個 zip。
3. 手機 App 用同一個帳號登入即可使用。
4. 沒有此功能的方案：把 [`news-fact-check-prompt.txt`](news-fact-check-prompt.txt) 的內容貼到對話開頭。

### ChatGPT
1. 新增 GPT，把 [`news-fact-check-prompt.txt`](news-fact-check-prompt.txt) 全文貼進「指示」。
2. 開啟網路搜尋功能。
3. 手機 App 登入同帳號即可使用。

### Gemini
1. 新增 Gem，把 [`news-fact-check-prompt.txt`](news-fact-check-prompt.txt) 全文貼進指示並儲存。
2. 手機 App 登入同帳號即可使用。

各平台的選單名稱與方案限制會變動，請以畫面為準。

## 怎麼使用
1. 輸入「查核」，並貼上連結、文字或截圖。
2. 看完每一步的結果後，輸入 `2`、`3`、`4`。
3. 想查下一則，直接貼上新內容。

## 重要限制
- 這是 AI 輔助判讀，**不取代專業查核**。請自行點開 Step 3 列出的來源網址確認。
- 需要 AI 能聯網搜尋。無法聯網時，它應該明說，不會假裝查過。
- AI 無法直接觀看影片，也無法自動做反向圖片搜尋；影片請提供文字描述或逐字稿。
- 查不到資料時會標示「查無」，不等於真或假。
- 各平台對「一次只輸出一個階段」的遵守程度可能不同。

## 授權
© 2026 budafang。本專案以 [CC BY 4.0](LICENSE) 授權：可自由使用、修改、散布與商用，使用時請標示原作者（budafang）與來源網址。

## 檔案
- `news-fact-check.zip`：Claude 技能包
- `news-fact-check-prompt.txt`：ChatGPT、Gemini 或其他 AI 用的純文字指示
- `skill/news-fact-check/SKILL.md`：Claude 技能原始檔
