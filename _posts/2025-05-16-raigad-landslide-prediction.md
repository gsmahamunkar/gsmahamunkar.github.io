---
layout: post
title: "Remote Sensing & ML for LULC in Raigad District"
date: 2025-04-24
---

# Landslide Susceptibility Prediction Using Machine Learning: A Case Study of Raigad District

---

## 🌍 Introduction

Landslides are a major natural hazard that can lead to loss of life, damage to property, and disruption of infrastructure. In regions like the Raigad district of Maharashtra, which lie in the Western Ghats with steep topography and high rainfall, landslides are a recurring concern, especially during the monsoon season.

This post summarizes the methodology and results of my research on landslide susceptibility prediction for the Raigad district using geospatial data and machine learning techniques.

---

## 🧭 Study Area: Raigad District, Maharashtra

Raigad is a coastal district located in the Konkan region, characterized by:

- **Geology**: A mix of sedimentary and basaltic igneous rocks prone to weathering and erosion.
- **Climate**: High monsoonal rainfall between June and September.
- **Topography**: Hilly terrain with steep slopes and fault lines.

The region has witnessed several devastating landslides in the past two decades. For instance:

| Event | Location | Date | Casualties |
|-------|----------|------|------------|
| Irshalwadi | July 19, 2023 | 26 dead, 109 missing |
| Taliye | July 22, 2021 | 89 dead |
| Dasgaon | July 25, 2005 | 48 dead |

---

## 📊 Data and Methodology

### ✅ Dataset Description

The study utilized field-collected data from **100 locations** in the Raigad district. Each data point was characterized using **7 key landslide conditioning factors**:

1. **Aspect**
2. **Curvature (plan and profile)**
3. **Elevation**
4. **NDVI (Normalized Difference Vegetation Index)**
5. **Precipitation**
6. **Land Use Land Cover (LULC)**
7. **Slope**

### 🧠 Machine Learning Approach

A **Multi-Layer Perceptron (MLP)** neural network was employed to predict landslide susceptibility. The MLP model was trained on the aforementioned parameters to classify sites as either susceptible or non-susceptible.

#### 📌 Why MLP?

- MLPs can capture complex non-linear relationships between features.
- They are well-suited for medium-sized tabular datasets.
- Once trained, the model is fast and efficient to deploy.

### 🗺️ Geospatial Tools

- **GIS (Geographic Information Systems)** was used to preprocess and visualize spatial data.
- **Remote Sensing** techniques were applied to derive vegetation and land use parameters.
- Integration of all data layers was carried out in a GIS environment to produce susceptibility maps.

---

## 🔍 Results & Observations

The trained MLP model was able to highlight regions of high susceptibility within the Raigad district. The model’s predictions aligned well with the locations of known historical landslides.

Key takeaways:

- Areas with **high slopes**, **low vegetation**, and **intense rainfall** were marked as high-risk zones.
- The model can serve as a basis for developing **early warning systems** and **zoning regulations**.

---

## 📌 Significance of the Study

- **Policy Making**: Helps local governments prioritize areas for slope stabilization and evacuation plans.
- **Disaster Mitigation**: Assists in preparing effective rescue and relief strategies.
- **Scalability**: The approach can be adapted to other regions with similar geographic characteristics.

---

## 🔭 Future Work

- Integrating **real-time rainfall data** for dynamic prediction.
- Expansion of the dataset using **crowdsourced incident reports**.
- Testing other ML models like Random Forest and Gradient Boosting for comparison.

---

## 📫 Connect With Me

If you're interested in geospatial data science, disaster risk management, or machine learning applications in the environment, let’s connect!  
🔗 [GitHub](https://github.com/gsmahamunkar) | 💼 [LinkedIn](https://linkedin.com/in/geetanjali-mahamunkar/)

---

*Note: This blog post is based on a chapter from my Ph.D. thesis focused on landslide prediction using machine learning for Raigad district.*
