# 紅酒品質預測分析
kaggle練習題，紅酒品質預測

資料欄位
1 - fixed acidity:固定酸度
2 - volatile acidity：揮發性酸度
3 - citric acid：檸檬酸
4 - residual sugar：殘糖
5 - chlorides：氯化物
6 - free sulfur dioxide：游離二氧化硫
7 - total sulfur dioxide：總二氧化硫
8 - density：密度
9 - pH：酸鹼度
10 - sulphates：硫酸鹽
11 - alcohol Output variable (based on sensory data):酒精輸出變量
12 - quality (score between 0 and 10)：品質(區分6.5以上是好，以下是壞）

敘述性分析
![image](https://github.com/barry80417/Prediction-of-quality-of-Wine/blob/main/%E7%B4%85%E9%85%92%E6%95%98%E8%BF%B0%E6%80%A7%E5%88%86%E6%9E%90.jpg)
敘述性分析發現，都沒有缺失值，但是每個數值欄位數字差異有點多，每個欄位數字差異有點大，數值範圍還要再做調整，還要將quality要區分好跟壞比較好做預測。
Fixed acidity、free sulfur dioxide、total sulfur dioxide、density、alcohol差異看起來比較大
quality在做區分好與壞之後，可以發現有資料不平衡的狀況，需要做調整


關聯性分析
![image](https://github.com/barry80417/Prediction-of-quality-of-Wine/blob/main/%E7%B4%85%E9%85%92%E5%93%81%E8%B3%AA%E9%97%9C%E8%81%AF%E5%9C%96.jpg)

分析完之後對內容進行清理，途中有多切一個欄位將quality>=7的切分為好品質，以下為壞品質，再對其進行labelencoding
此份資料沒有空職需要處理，比較有資料不平衡問題

之後對其進行隨機森林、KNN模型、決策數、向量機、XGBoost及keras模型練習
