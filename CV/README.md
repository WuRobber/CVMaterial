# 📌 電腦視覺與應用專案說明

## 📝 期中專案說明  
本專案模擬基於已知結構的 3D 掃描裝置場景。在虛擬環境中，一個 3D 物體位於 200 mm 寬的立方框架內。我們假設有一個與立方體側面平行的平行光源（如太陽）。給定的影像是透過在光源前插入一根桿子來渲染的，因此投射的陰影將是物體與平面的交點，如下圖所示：  
![Figure](../Image/CV-A_src1.png)  

### 📂 期中專案資源  
#### 🔹 程式碼  
- **主要程式碼：**  
  - [`MidtermProject.ipynb`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/MidtermProject/MidtermProject.ipynb)  

#### 🔹 專案報告  
- [`R12522636_MidtermReport.pdf`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/MidtermProject/R12522636_MidtermReport.pdf)  

#### 🔹 最終輸出  
- **座標文件：**  
  - [`R12522636.xyz`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/MidtermProject/R12522636.xyz)  

📌 **更多細節請參閱**：[MidtermProject 資料夾](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/MidtermProject)  

---

## 📝 期末專案說明  
本專案的目標是透過立體視覺（stereoscopic images）重建 3D 點雲。影像的內部與外部參數已提供於 `CameraParameter.txt`，需要撰寫程式導入並分析左右影像序列，最終輸出 `.xyz` 格式的彩色 3D 座標文件。  

### 🎯 核心步驟  
1. **影像分割**：將每幀影像拆分為左、右兩張影像。  
2. **特徵點匹配**：在左影像每行選擇最亮像素（根據藍色通道辨識），尋找右影像中的對應點，並依據極線幾何約束驗證其正確性。  
3. **3D 點雲計算**：使用「直接三角測量（Direct Triangulation）」計算 3D 座標。  
4. **誤差排除**：透過重投影誤差（Re-projection Error）過濾異常點。  
5. **結果存儲**：將 `X Y Z RGB` 格式的數據存入 `.xyz` 文件，可透過 MeshLab 可視化點雲。  

#### 🔹 立體影像與點雲可視化  
![Figure](../Image/CV-A_src2.png)  
![Figure](../Image/CV-A_src3.png)  

### 📂 期末專案資源  
#### 🔹 程式碼  
- **主要程式碼：**  
  - [`main.ipynb`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/FinalProject/main.ipynb)  

#### 🔹 專案報告  
- [`R12522636_FinalReport.pdf`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/FinalProject/R12522636_FinalReport.pdf)  

#### 🔹 最終輸出  
- **座標文件：**  
  - [`R12522636.txt`](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/FinalProject/R12522636.txt)  

📌 **更多細節請參閱**：[FinalProject 資料夾](https://github.com/WuRobber/CVMaterial/blob/main/CV-A/FinalProject)  
