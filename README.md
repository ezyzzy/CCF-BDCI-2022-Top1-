# CCF-BDCI-2022-返乡发展人群预测赛题-Baseline
CCF BDCI 2022比赛 返乡发展人群预测赛题 Baseline 数据挖掘（特征工程+集成学习）队伍排名39/2297  
比赛链接：https://www.datafountain.cn/competitions/581  
> 该赛题是数据挖掘问题，通过使用中国联通所提供的包括信令、通话、互联网行为等数据建立分类模型，对个人是否会返乡工作进行二分类判断。  

### 数据理解
feature 47 {index: 1, 位置类特征(cls, int): 6, 互联网特征(int): 37, 通话类特征(int): 4}, y 1  
Train 6e4  
TrainNoLabel 4e4  
TestA/B 5e4/5e4  
  
### 特征工程
1. 序号编码
2. 特征组合
3. 数据清洗
4. 特征选择
  
### 集成学习
1. 模型选择GBDT: XGBoost, LGBM, CatBoost
2. Stacking
3. Bagging
4. Grid Search: hyper parameters tunning
  
### 半监督学习（弃用）
1. 预测无标签训练集数据
2. 设置置信度阈值筛选数据，和原有训练集合并
  
离线结果 (AUC: 0.9103)，在线Test A (AUC: 0.9120)，在线Test B (AUC: 0.8994)
