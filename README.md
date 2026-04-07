# 🏥 AI-Based Disease Prediction System
### MCA Final Year Project | Complete Google Colab + Streamlit Deployment

---

## 📁 Project Structure

```
AI_Disease_Prediction_System_MCA.ipynb   ← Main notebook (upload to Colab)
```

---

## 🚀 How to Run (Step-by-Step)

### Step 1 — Upload to Google Colab
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Upload Notebook**
3. Select `AI_Disease_Prediction_System_MCA.ipynb`

### Step 2 — Run Cells in Order

| Cell | Purpose | Time |
|------|---------|------|
| **Cell 1** | Install all Python packages | ~1 min |
| **Cell 2** | Generate dataset (3000 rows, 15 diseases, 42 symptoms) | ~5 sec |
| **Cell 3** | Train & compare 4 ML models, save best model | ~3 min |
| **Cell 4** | Quick prediction sanity check | ~5 sec |
| **Cell 5** | Write Streamlit app code to disk | ~2 sec |
| **Cell 6** | Launch app + ngrok → prints public URL | ~15 sec |

---

## 🤖 Machine Learning Details

### Models Trained
| Model | Notes |
|-------|-------|
| Logistic Regression | Baseline linear classifier |
| Decision Tree | Interpretable tree-based model |
| **Random Forest** | **Usually selected as best model** |
| SVM (RBF kernel) | Kernel-based classifier |

### Evaluation Metrics
- Accuracy, Precision, Recall, F1 Score
- 5-Fold Cross-Validation
- Confusion Matrix
- Classification Report

### Dataset
- **15 diseases** × **42 symptoms** × **200 samples** = **3,000 rows**
- Domain-knowledge-based symptom profiles (primary + secondary symptoms)
- Realistic probabilistic noise injection

---

## 🌐 Web App Features

### Sidebar
- 42 symptoms organized into 8 medical categories
- Expandable category sections
- Real-time symptom count badge
- One-click prediction button

### Results Tabs
1. **📋 Recommendations** — Precautions, diet, medications, emergency guidance
2. **📊 Analysis** — Confidence gauge, probability bar chart, selected symptoms
3. **🏆 Top-3 Diagnoses** — Top 3 most likely conditions with confidence
4. **📈 Model Stats** — Comparison chart and performance table

### Severity System
| Badge | Color | Diseases |
|-------|-------|---------|
| 🟢 LOW RISK | Green | Common Cold, Migraine, Chickenpox |
| 🟡 MODERATE RISK | Orange | Influenza, Bronchitis, Diabetes, Hypertension |
| 🔴 HIGH RISK | Red | COVID-19, Pneumonia, Malaria, Dengue, Typhoid, Hepatitis B, TB |
| 🚨 CRITICAL | Purple | Meningitis |

---

## 🏥 Diseases Covered (15)
Common Cold • Influenza • COVID-19 • Pneumonia • Bronchitis  
Malaria • Dengue Fever • Typhoid • Hepatitis B • Tuberculosis  
Diabetes • Hypertension • Migraine • Chickenpox • Meningitis

---

## 📊 Symptoms Covered (42)
**Fever & Systemic:** fever, high_fever, chills, fatigue, malaise, sweating, weight_loss, weight_gain  
**Pain:** headache, body_ache, joint_pain, muscle_pain, back_pain, chest_pain, stomach_pain  
**Respiratory:** cough, dry_cough, productive_cough, shortness_of_breath, sore_throat  
**ENT:** runny_nose, nasal_congestion, sneezing, loss_of_smell, red_eyes  
**GI:** nausea, vomiting, diarrhea, loss_of_appetite, dark_urine, clay_colored_stool  
**Skin:** skin_rash, itching, yellowish_skin, pale_skin  
**Neurological:** dizziness, blurred_vision, stiff_neck, sensitivity_to_light  
**Metabolic:** excessive_thirst, frequent_urination, swollen_lymph_nodes

---

## ⚕️ Medical Disclaimer
> This system is developed for **educational and academic purposes only**. It is not a substitute for professional medical diagnosis or treatment. Always consult a qualified and licensed physician for medical advice.

---

## 📝 Project Info
- **Domain:** Healthcare AI / Medical Informatics
- **Stack:** Python · scikit-learn · Streamlit · ngrok · Plotly · Seaborn
- **Deployment:** Google Colab + ngrok public tunneling
- **Model Storage:** pickle serialization
