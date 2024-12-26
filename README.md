# Node.js S3 Order Management

## 簡介
此專案是一個使用 Node.js 和 AWS SDK v3 的應用程序，旨在從 Amazon S3 存儲桶中讀取和更新訂單數據。該應用程序允許使用者新增訂單並將其存儲到 S3 中，便於管理和持久化訂單資料。

## 功能
- 從指定 S3 桶中讀取訂單資料。
- 解析訂單請求並新增訂單。
- 更新 S3 中的訂單 JSON 文件。
- 處理錯誤並返回相應的狀態碼。

## 安裝與使用方式
1. 確保您已安裝 [Node.js](https://nodejs.org/) 環境。
2. 克隆這個儲存庫：
   ```bash
   git clone https://github.com/your-username/repo-name.git
   cd repo-name
   ```
3. 安裝必要的依賴模組：
   ```bash
   npm install @aws-sdk/client-s3 moment
   ```
4. 更新以下變數以適應您的 AWS 設定：
   - `BUCKET_NAME` (S3 桶名)
   - `FILE_NAME` (檔案名)
   - `region` (AWS 区域)
   - `accessKeyId` (AWS 存取金鑰)
   - `secretAccessKey` (AWS 私密金鑰)

5. 當訂單請求準備就緒時，可以執行此函數來新增訂單。範例：
   ```javascript
   main(`{"orderName":"Test Order","description":"Test Description","products":[{"id":"ks001","qty":4}]}`
   ```

## 必要的依賴模組清單
- `@aws-sdk/client-s3`: AWS SDK for JavaScript，用於與 Amazon S3 互動。
- `moment`: 處理和格式化日期的輕量級庫。

## 授權條款
本專案遵循 [MIT 授權](LICENSE)。請隨時查閱相關檔案以獲取更多資訊。
```

請根據您的 GitHub 用戶名稱和儲存庫名稱替換 `your-username/repo-name`，並確保將授權條款的細節正確反映在 LICENSE 檔案中。