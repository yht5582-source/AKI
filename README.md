# AKI 急性腎損傷臨床導航

繁體中文成人 AKI 互動網頁，將診斷與分期、病因排查、透析啟動、模式選擇，以及脫離透析評估串成連續流程，供醫療人員臨床討論與教學使用。

**版本：v1.0｜指引查核日期：2026-11-26**

- 儲存庫：[yht5582-source/AKI](https://github.com/yht5582-source/AKI)
- GitHub Pages 預定網址：[https://yht5582-source.github.io/AKI/](https://yht5582-source.github.io/AKI/)
- 發布狀態：本版交付時尚未完成 GitHub Pages 發布確認；預定網址不代表已上線。

## 適用對象與範圍

適用於 **18 歲以上成人 AKI** 的評估與教學。兒童、孕產婦、慢性維持性透析及特殊中毒，須使用相應專科路徑。

本工具不是經前瞻性驗證的決策模型，也不是學會認證演算法，不自動開立醫囑。輸出須由照護醫師結合病程、治療反應、照護目標及可用資源確認。

## 主要功能

| 流程 | 功能 |
| --- | --- |
| 病人資料 | 整合具有時間條件的肌酐變化、可靠的連續尿量及無尿時間，判定 KDIGO AKI 分期並顯示理由。 |
| 病因排查 | 提供體液流失、感染、鬱血、阻塞、腎小管損傷、藥物、腎絲球炎、間質炎、橫紋肌溶解、TMA 及肝病等線索與優先行動。 |
| 透析時機 | 逐項確認高血鉀、難治酸中毒、低氧性容量過多、尿毒併發症及符合體外清除適應症的中毒；非緊急情境再評估腎臟能力與病人需求。 |
| 模式選擇 | 依循環、腦損傷、快速清除需求、血鈉異常及資源，提供 IHD、CRRT／CKRT、SLED／PIRRT 與急性 PD 的條件式方向。 |
| 脫離透析 | 整合病因改善、循環、容量、代謝、尿量、利尿劑及定時尿液 CrCl，判斷是否具備監測下試停的條件。 |

其他功能包括即時決策摘要、8 個虛構示範病例、CRRT effluent 教學換算、可列印整合摘要，以及指引來源連結。

## 使用方式

1. 開啟網頁，輸入成人年齡、肌酐及尿量資料；確認每筆資料的時間與可信度。
2. 選擇目前存在的病因線索，依提示完成基本排查。未勾選不代表已排除。
3. 在「透析時機」逐項選擇「是／否／尚未確認」。遇到生命威脅時立即處置，不等待表單完成。
4. 如需 RRT，在「模式選擇」補齊臨床條件，查看方向、限制與衝突提醒。
5. 正因 AKI 接受 RRT 者，可於「脫離透析」檢視恢復條件，並規劃監測及重啟安排。
6. 使用「列印摘要」產生整合報告；可透過瀏覽器另存 PDF。

可從上方步驟自由切換。載入示範病例會取代目前輸入，載入後可修改資料觀察決策變化。

### 單位與輸入注意事項

- 血清與尿液肌酐均使用 **mg/dL**。
- 血鉀及 HCO₃⁻ 使用 **mmol/L**；BUN 使用 **mg/dL**，不要直接填入 urea 濃度。
- 分期用尿量為 **mL/kg/h**，須符合連續時段與收集可信度要求，不能直接套用任意 24 小時平均值。
- 恢復評估的 24 小時尿量使用 **mL/day**；CrCl 的收集尿量則是本次定時收集總量。
- 空白與「尚未確認」不視為正常或已排除。超出有效輸入範圍時，介面暫停決策輸出並要求修正。

## 判讀原則

- AKI 第 3 期不等於必須立即透析；肌酐、BUN 或 eGFR 不能單獨決定啟動或停止 RRT。
- 尚未排除緊急適應症時，不顯示可嘗試脫離透析的結論。
- 尿量增加不等於溶質清除恢復，尤其使用利尿劑時需整合其他證據。
- 定時尿液 CrCl 是估計值，受收集完整性、血清肌酐變動及 RRT 干擾影響；不校正至 1.73 m²。
- 本工具中的部分數值用於危險提示、研究情境重評或保守的一致性檢查，不應一律解讀為學會通用的啟動／停機門檻。其意義與限制已標於對應畫面。
- CRRT 轉換為 IHD 或 SLED 仍屬透析支持，不代表脫離 RRT。
- CRRT effluent 代表治療清除劑量的相關流量，不等於病人淨除水量；本頁不直接產生完整透析處方。

## 示範病例

1. 缺水型 AKI，可先處理病因。
2. 敗血性休克與肺水腫。
3. 阻塞合併感染。
4. 高血鉀合併心電圖變化。
5. AKI 恢復，可討論監測下試停。
6. 利尿後尿量多，但清除仍不足。
7. 慢性高肌酐，急性證據不明。
8. 腦損傷合併快速清除需求。

病例均為虛構資料，用於教學與功能演示。

## 本機開啟與 GitHub Pages 部署

### 本機使用

網頁為單一 HTML 檔，內含 CSS 與 JavaScript，不需安裝套件、API 金鑰或資料庫。下載 `index.html` 後，以瀏覽器開啟即可操作；查閱外部指引連結時需要網路。

### 儲存庫檔案

| 檔案 | 用途 |
| --- | --- |
| `index.html` | 網站首頁與全部互動功能；部署時放在儲存庫根目錄。 |
| `README.md` | 專案介紹、操作與部署說明。 |

開發工作目錄中的 `dist/index.html`，上傳至本儲存庫時應放在根目錄，命名為 `index.html`。

### 啟用 Pages

1. 將 `index.html` 與 `README.md` 上傳至 `yht5582-source/AKI` 的 `main` 分支。
2. 開啟儲存庫的 **Settings → Pages**。
3. 在 **Build and deployment** 將 Source 設為 **Deploy from a branch**。
4. 將 Branch 設為 **main**、資料夾設為 **/ (root)**，按 **Save**。
5. 等待 Pages 部署工作完成，再開啟預定網址並確認頁面與按鈕功能。

儲存庫名稱與網址中的 `AKI` 請保留原大小寫。若出現 404，先檢查 Pages 部署狀態、分支與首頁位置。

## 資料處理

- 本版未設後端、病歷介接或分析追蹤程式。
- 表單資料保留於目前頁面記憶體；重新整理或關閉頁面後不保留。
- 不收集姓名與病歷號。
- 列印或另存 PDF 會產生使用者自行保管的報告，請依院內資料管理規範處理。

## 驗證狀態與限制

已完成 **58 項程式與邏輯檢查**，涵蓋分期邊界、慢性高肌酐、缺失資料、緊急警示、模式衝突、CrCl、利尿劑影響、試停攔阻，以及示範病例各步驟的程式輸出。

檢查使用 Node.js 執行邏輯與簡化 DOM 替身，並完成靜態 HTML ID 重複檢查。這些結果不等同於真實瀏覽器、手機、列印版面驗證或臨床有效性驗證。本版交付時，環境限制使上述實際瀏覽器驗證與線上發布確認尚未完成。

正式納入院內流程前，仍需由腎臟科與重症團隊覆核分支內容、監測安排、設備資源及特殊族群處理方式。

## 指引與原始研究

1. **KDIGO Clinical Practice Guideline for Acute Kidney Injury（2012）**：AKI 定義與分期、病因評估、啟動／停止 RRT、模式及劑量。 [全文 PDF](https://kdigo.org/wp-content/uploads/2016/10/KDIGO-2012-AKI-Guideline-English.pdf)
2. **NICE NG148（2024 更新）**：AKI 評估、尿液檢查、阻塞影像與轉介。 [Recommendations](https://www.nice.org.uk/guidance/ng148/chapter/Recommendations)
3. **ISCCM Guidelines on Acute Kidney Injury and Renal Replacement Therapy（2022）**。 DOI: `10.5005/jp-journals-10071-24109`。 [全文](https://pmc.ncbi.nlm.nih.gov/articles/PMC9989875/)
4. **STARRT-AKI — Timing of Initiation of Renal-Replacement Therapy in Acute Kidney Injury（NEJM 2020）**。 DOI: `10.1056/NEJMoa2000741`。 [PubMed](https://pubmed.ncbi.nlm.nih.gov/32668114/)
5. **AKIKI 2 — Comparison of two delayed strategies for renal replacement therapy initiation for severe acute kidney injury（Lancet 2021）**。 DOI: `10.1016/S0140-6736(21)00350-0`。 [PubMed](https://pubmed.ncbi.nlm.nih.gov/33812488/)
6. **ISPD guidelines for peritoneal dialysis in acute kidney injury: 2020 update（adults；2021 刊行）**。 DOI: `10.1177/0896860820970834`。 [PubMed](https://pubmed.ncbi.nlm.nih.gov/33267747/)
7. **EXTRIP Workgroup**：毒物別體外清除建議。 [Recommendations](https://www.extrip-workgroup.org/recommendations)

截至本版查核，新版 KDIGO AKI／AKD 文件仍有公開審閱草案標示，本版未將草案建議當作正式指引規則。正式更新發布後，應重新審查相關分支。 [KDIGO 更新頁面](https://kdigo.org/guidelines/acute-kidney-injury/)

## 版本紀錄

### v1.0 — 2026-11-26

- 建立五步連續評估流程與即時決策摘要。
- 加入缺失資料、危險數值及試停條件攔阻。
- 提供 8 個教學病例、CrCl 計算、CRRT effluent 教學換算及列印摘要。
- 附正式指引與原始研究來源，標示草案與驗證限制。
