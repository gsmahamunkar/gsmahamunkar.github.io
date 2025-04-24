---
layout: post
title: "LULC Mapping of Raigad District Using Random Forest and Sentinel-2 Data"
date: 2025-04-24
---


## 🌿 Mapping Land Use Land Cover of Raigad District Using Random Forest: A Remote Sensing Approach

---

### 📌 Introduction

Monitoring land use and land cover (LULC) is essential for managing natural resources and understanding environmental dynamics, especially in regions like **Raigad district, Maharashtra**, where urban growth meets rich biodiversity. In this post, I highlight part of my doctoral research where I applied **Remote Sensing and Machine Learning** to classify LULC using the **Random Forest algorithm**.

---

### 📍 Study Area: Raigad District

Located in the **Konkan region of Maharashtra**, Raigad features a varied landscape of coastal areas, hilly ranges, rivers, and growing urban zones. This diversity makes it a valuable case study for land cover mapping.

---

### 🛡️ Data Used

- **Satellite Data:**  
  - **Sentinel-2A imagery (Level-1C)**  
  - Date of acquisition: **January 2022**
  - Processed to **surface reflectance (Level-2A)** using **Sen2Cor**

---

### 📊 Methodology Overview

#### 🔍 1️⃣ Preprocessing
- **Atmospheric correction** with **Sen2Cor**
- **Cloud masking** applied
- **Band selection:** All 10m and 20m bands (resampled to 10m resolution)

#### 🌲 2️⃣ LULC Classification Using Random Forest

A **Random Forest classifier** was trained and applied in **Google Earth Engine (GEE)** to categorize the land cover into four distinct classes:

1. **Built-up**
2. **Vegetation**
3. **Waterbody**
4. **Other**

- **Training Data:** Derived from field-collected points, satellite interpretation, and ancillary records.
- **Classifier Parameters:**  
  - Number of trees: **100**
  - Features per split: **sqrt**

#### 🗺️ 3️⃣ Accuracy Assessment
The classification's performance was evaluated using an **independent validation dataset** and a **confusion matrix**.

- **Overall Accuracy:** **84.49 %**
---

### 🌾 LULC Classification Results

The final LULC map revealed:
- Extensive **vegetation cover** over forested and hilly terrain.
- Increasing **built-up areas** near industrial corridors and urban centers.
- Clearly demarcated **water bodies** including rivers, lakes, and reservoirs.
- **Other** areas, covering miscellaneous land uses not classified in the other three categories.

#### 📷 Example Output:  

![LULC Classification Map of Raigad District](/images/RaigadLULC2002-21.png)


---

### 📌 Conclusion

This study demonstrates how freely available **Sentinel-2 data** and **Random Forest machine learning techniques** on **Google Earth Engine** can be effectively used for accurate and scalable LULC mapping in environmentally and economically important regions like Raigad.

---
