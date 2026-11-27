# 🥃 YourDrinksPalate — A Spirit & Cocktail Recommender & Taste Predictor

**YourDrinksPalate** is an interactive mobile application mockup designed to help users discover both neat spirits (straight drinks) and craft cocktails tailored to their personal sensory profile, while predicting how much they will enjoy any bottle or drink before ordering.

## 🌟 Novelty & Core Value Proposition
Existing beverage apps focus either on static recipe catalogs (e.g., Cocktail Flow) or crowdsourced wine/beer ratings (e.g., Vivino, Untappd). **YourDrinksPalate** bridges the gap between neat spirits and mixed cocktails by modeling—and continuously adapting—the user's sensory palate across **5 distinct flavor dimensions**:
1. **Sweetness** (Rich / Caramel)
2. **Acidity / Citrus** (Crisp / Tart)
3. **Bitterness** (Amaro / Oak Tannin)
4. **Smokiness / Peat** (Charred Barrel / Smoke)
5. **Herbal / Botanical** (Spice / Anise)

## 🧠 Course Functional Requirements Covered

### 1. Recommender System (Tab 1: Flavor DNA & Tab 2: Discover)
* **Sensory Vector Profiling & Live Radar:** Users configure their 5D Taste Vector via interactive sliders or quick presets, visualized in real time on a 5-axis SVG radar chart.
* **Hybrid Similarity Matching:** The recommender engine compares the user's effective 5D taste vector against a curated dataset of **12 beverages** (6 Neat Spirits & 6 Craft Cocktails) using a weighted Cosine Similarity and Euclidean distance blend to compute a real-time **Match Percentage (`% Match`)**.
* **Multi-Dimensional Filtering & Live Search:**
  * **Instant Search Bar:** Search across drink names, tasting notes, and ingredients in real time.
  * **Drink Format:** Filter by *All*, *Neat Spirits (Σκέτα Ποτά)*, or *Craft Cocktails*.
  * **Spirit Base:** Filter by *Whisky*, *Rum*, *Tequila/Mezcal*, *Gin*, *Vodka*, and *Tsipouro*.
  * **Alcohol Strength (ABV):** Filter by *Light (<22%)*, *Medium (22–39%)*, or *High Proof (40%+)*.
  * **Occasion & Mood:** Filter by *Summer & Refreshing*, *Aperitivo*, *After-Dinner Sipper*, or *Bold & Night Out*, plus a quick toggle for *Saved Favorites*.
* **Full At-a-Glance Card Details:** Every beverage card in the ranked list displays its key ingredients, tasting notes, ABV%, and occasion tags directly without requiring extra clicks.
* **Desktop & Mobile Navigation:** Horizontal filter bars include quick-scroll arrow controls (`‹` / `›`) and mouse-wheel support alongside touch scrolling.

### 2. Predictive Model & Closed-Loop Learning (Tab 3: AI Predictor)
* **Personal Taste Rating Predictor (`1.0 – 5.0 ★`):** Before ordering an unfamiliar spirit or cocktail, the model predicts the exact rating the user will give it, complete with a **Dual Radar Overlay** (User DNA vs. Drink Profile) and **Explainable AI** feature attribution bars.
* **"What-If" Serving Style Simulator:** Users can dynamically test how changing the serving style (*Neat / Σκέτο*, *On the Rocks / Με Πάγο*, *With Citrus Twist*, *Splash of Water*) alters bitterness, smoke, and citrus acidity—updating the Predicted Rating in real time.
* **Favorites, Ratings & Closed-Loop Palate Learning:** Users can bookmark favorite drinks (`♥`) and log personal ratings (`1–5 ★`) persisted via `localStorage`. High-rated and saved drinks dynamically shift the user's effective 5D taste vector, updating match scores and overlaying the learned palate shift onto the Flavor DNA radar chart.

## 🚀 How to Run the Interactive Mockup
1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser (Chrome, Safari, Firefox, Edge). No build step or external server is required.
