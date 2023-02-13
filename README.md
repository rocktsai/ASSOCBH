# ASSOCBH
AI-assisted sentencing system for Offenses of Causing Bodily Harm<br>
由人工智慧輔助的傷害罪量刑系統
## 動機
1. 實任司法官養成曠日廢時
2. 案件數量越來越多
## 目的
1. 減輕法官作審案時間、提升法院效率
2. 檢察官及律師可以參考模型給出的判決結果
## 為什麼選擇傷害罪?
  傷害罪是刑法中較基礎的犯罪 <br>
  傷害罪的案件佔比高
## 專案流程簡介
1. 利用Python Selenium等套件進行大量判決書文本爬取
2. 利用Python Pandas等套件進行文本的清整與資料集的建立
3. 架設Hadoop分散式檔案系統並用Spark進行後續資料集的處理
4. 利用jieba、word2vec、TF-IDF搭配人工篩選機制進行特徵工程
5. 利用隨機森林與xgboost將encoding後的資料及進行訓練
6. 利用HTML搭配Flask將訓練好的模型串接上網頁
7. 利用Docker將網頁部署上AWS
