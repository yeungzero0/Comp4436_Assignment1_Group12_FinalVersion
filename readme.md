# COMP4436 Assignment 1  
Group member:  
Yeung Hang (22027226d) [me]  
Yeung Tsz Kwan (23103029d)   
Chan Kin Wang (23031551d)  
**Comparative Analysis of ML, DL and SNN Algorithms for Cat vs Dog Image Classification**

[![Python](https://img.shields.io/badge/Python-3.9-blue)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://www.tensorflow.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-green)](https://scikit-learn.org/)

這是 **POLYU COMP4436 Artificial Intelligence of Things (AIoT)** 的 Group Assignment 1。  
我們比較了 **五種演算法** 在貓狗圖像分類任務上的性能，包含：

- **Machine Learning**：Logistic Regression (Supervised)、K-Means (Unsupervised)
- **Deep Learning**：CNN (Supervised)、Autoencoder (Unsupervised)
- **Hybrid**：**SNN × CNN**（Spiking Neural Network 使用 CNN 特徵提取）

**最佳模型**：**SNN × CNN**，在測試集上達到 **Accuracy ≈ 0.8707**，大幅優於其他模型。

---

## ⚠️ 免責聲明 (Disclaimer)

**本專案純粹用於學習與課程用途**。

- 此專案是 **POLYU COMP4436 Group 12(2025)** 的作業，主要目的是比較傳統 ML、DL 與 SNN 在 AIoT 應用中的表現。
- **嚴禁商業使用**：本專案**不得**用於任何商業活動、產品開發或生產環境。
- **僅供參考與教育**：所有程式碼、結果與報告僅供個人學習、測試與參考之用。
- **無任何保證**：作者不對使用本專案所產生的任何輸出、結果或後果承擔任何責任。

> **總之：這只是我們在 POLYU 學習 AIoT 與神經網路的課程作業，不是專業解決方案。**

---

## 專案特色

- 使用 **Cats & Dogs Image Classification Dataset**
- 涵蓋 **Supervised + Unsupervised** 兩種學習方式
- 包含 **ML、DL、SNN** 三類演算法
- 完整比較 **Accuracy、Precision、Recall、F1-Score、Execution Time**
- **SNN × CNN** 結合 CNN 特徵提取與 SNN 脈衝神經網路，展現 AIoT 應用潛力（能量效率高、即時處理、噪音容忍度佳）


![image](https://github.com/yeungzero0/Comp4436_Assignment1_Group12_FinalVersion/blob/main/CatDog2025_Timg.png)

---

## 如何運行專案

### 1. 環境需求
- Python **3.9.x**（推薦使用官方 3.9 版本）
- VSCode + Python 擴充套件

### 2. 環境設定步驟（詳細請見 `readme.txt`）
1. 安裝 Python 3.9.x（[官方下載](https://www.python.org/downloads/)）
2. 打開 VSCode，將專案資料夾 **Comp4436_Assignment1_Group12** 拖入 VSCode
3. 打開 `All_algorithm.ipynb`（包含所有 5 種演算法）
4. 按 **F1** 選擇 Python 3.9.x 作為 interpreter
5. 在 VSCode 終端機（Ctrl + `）執行以下指令安裝所需套件：


---  
Setup python and VsCode  
1.ensure the python is 3.9.x Version (if not install 3.9.x, go to "https://www.python.org/downloads/" and find 3.9.x Version  
2.open your VsCode  
3.drag and drop the project file "Comp4436_Assignment1_Group12" into the VsCode  
4.open the "All_algorithm.ipynb" or each .ipynb files (All_algorithm.ipynb including all 5 algorithml: LR, K-Means, PCA, CNN, SNN)  
5.scroll down and see the result at "All_algorithm.ipynb" or each .ipynb files  
6.Press F1 and select the python 3.9.x (ensure the VsCode has be downloaded the python extension)  
  
If you run by yourself, install lib by using pip  
7.open the terminal (VsCode hot key: Ctrl + `)  
8.Enter "pip install --user --upgrade pip" in terminal (if can't install, also try to add "python -m " before the "pip inst...")  
9.Enter "pip install numpy opencv-python pandas seaborn tensorflow matplotlib scikit-learn scikit-image keras nengo python-time" in terminal  
10.Click "Run All" (if you are ready download the python extension, you can see the button on the top)  
  
