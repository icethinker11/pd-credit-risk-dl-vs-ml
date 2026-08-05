# PD Credit Risk: Deep Learning vs. Machine Learning
 
Modelado de la Probabilidad de Incumplimiento (PD, *Probability of Default*) — el componente central del riesgo crediticio — comparando el rendimiento e interpretabilidad de deep learning frente a modelos clásicos de machine learning.
 
![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 🎯 Motivación
  
El riesgo crediticio se descompone tradicionalmente (bajo el marco de Basilea) en tres componentes: **PD** (Probability of Default), **LGD** (Loss Given Default) y **EAD** (Exposure at Default). Este proyecto se enfoca específicamente en el modelado de **PD**: la probabilidad de que un cliente incumpla con el pago de su crédito.
 
Existe la creencia generalizada de que el deep learning supera automáticamente a los métodos "clásicos" de machine learning. Sin embargo, la literatura reciente sobre datos tabulares sugiere que modelos como el gradient boosting (XGBoost, LightGBM) suelen igualar o superar a redes neuronales en este tipo de problemas.
 
Este proyecto pone a prueba esa hipótesis en un caso real de modelado de PD, comparando deep learning con un conjunto de modelos de machine learning y evaluando no solo el rendimiento predictivo, sino también la interpretabilidad de cada enfoque, lo cual es un factor crítico en la industria financiera, donde los reguladores exigen explicabilidad en las decisiones de crédito.
 
**Pregunta de investigación:** ¿Justifica la complejidad adicional del deep learning su uso frente a machine learning clásico en un modelo de PD con datos tabulares?
 
**Nota de alcance:** este proyecto modela únicamente el componente PD del riesgo crediticio. 

## 📊 Dataset
 
[Default of Credit Card Clients Dataset](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset) (UCI / Kaggle) — 30,000 clientes de tarjetas de crédito en Taiwán (2005), con 23 variables predictoras (demográficas, historial de pago de 6 meses, montos facturados y pagados) y una variable objetivo binaria (incumplimiento el mes siguiente).
