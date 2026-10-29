# 🥃 YourDrinksPalate — A Spirit & Cocktail Recommender & Taste Predictor

**YourDrinksPalate** is an interactive mobile application mockup designed to help users discover both **neat spirits (straight drinks)** and **craft cocktails** tailored to their personal sensory profile, while predicting how much they will enjoy any bottle or drink before ordering.

---

## 🌟 Novelty & Core Value Proposition
Existing beverage apps focus either on static recipe catalogs (e.g., *Cocktail Flow*) or crowdsourced wine/beer ratings (e.g., *Vivino*, *Untappd*). **YourDrinksPalate** bridges the gap between **neat spirits** and **mixed cocktails** by modeling the user's sensory palate across 5 distinct flavor dimensions:
1. **Sweetness**
2. **Acidity / Citrus**
3. **Bitterness**
4. **Smokiness / Peat**
5. **Herbal / Botanical**

---

## 🧠 Course Functional Requirements Covered

### 1. Recommender System (`Tab 1: Flavor DNA` & `Tab 2: Discover`)
* **Sensory Vector Profiling:** Users configure their 5D Taste Vector via interactive sliders (or quick presets) and select their preferred spirit bases.
* **Cosine Similarity Matching:** The recommender engine compares the user's normalized 5D taste vector against a dataset of **12 beverages** (6 Neat Spirits & 6 Craft Cocktails), computing a real-time **Match Percentage (`% Match`)**.
* **Dual-Layer Filtering:** Users can filter recommendations by **Drink Format** (*All*, *Neat Spirits / Σκέτα Ποτά*, *Craft Cocktails*) and by **Spirit Base** (*Whisky/Scotch*, *Rum*, *Tequila & Mezcal*, *Gin*, *Vodka*, *Tsipouro & Aperitivo*), whether served straight or as a cocktail base.

### 2. Predictive Model (`Tab 3: AI Predictor`)
* **Personal Taste Rating Predictor (`1.0 – 5.0 ★`):** Before ordering an unfamiliar spirit or cocktail, the model predicts the exact rating the user will give it based on sensory alignment and historical preferences.
* **"What-If" Serving Style Simulator:** Users can dynamically test how changing the serving style (*Neat / Σκέτο*, *On the Rocks / Με Πάγο*, *With Citrus Twist*, *Splash of Water*) alters the chemical dilution, temperature, and acidity—updating the **Predicted Rating** in real time.

---

## 🚀 How to Run the Interactive Mockup
1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser (Chrome, Safari, Firefox, Edge). No build step or external server is required.
