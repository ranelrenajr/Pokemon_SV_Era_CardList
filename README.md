# Scarlet & Violet Pokémon TCG Data

This repository contains **scraped and structured data** of all playable cards from the **Pokémon Scarlet & Violet Base Set** (cards #001–198).
The goal of this project is to provide an easy-to-use dataset for research, deck building, data analysis, and hobby projects related to the Pokémon Trading Card Game (TCG).

---

## 📂 Repository Contents

* `data/` – Raw and cleaned data of cards from the SV Base set.
* `Scarlet_and_violet_base_set.json` – Full dataset in JSON format.

Each card entry typically includes:

* **Card number** (e.g., SV 045/198)
* **Name** (Pokémon / Trainer / Energy)
* **Card type** (Pokémon, Trainer, Energy)
* **Sub-type** (Basic, Stage 1, Supporter, Item, etc.)
* **HP / Attack(s) / Cost(s)** (for Pokémon)
* **Rules text / Effects**
* **Set info**

---

## 🚀 Usage

You can use the dataset for:

* Building **deck analysis tools**
* Running **card frequency studies**
* Creating **searchable databases** or web apps
* Training **machine learning models** on TCG text data

Example (Python):

```python
import json

with open("data/cards_001-198.json", "r", encoding="utf-8") as f:
    cards = json.load(f)

# Print the first card
print(cards[0])
```

---

## 🛠️ How the Data Was Collected

* Cards were **scraped from online sources** containing Pokémon TCG data.
* Focused on **playable attributes** only (flavor text, artwork, rarity, etc. may not be included).
* Cleaned and normalized into a structured format for easier use.

---

## 📅 Current Progress

* ✅ Scarlet & Violet Base Set **001–198** complete
* 🔜 Future expansions from the Scarlet & Violet era will be added

---

## ⚠️ Disclaimer

* This project is **fan-made** and not affiliated with, endorsed by, or sponsored by *The Pokémon Company International*.
* Data is provided **for research and educational purposes only**.
* Please support the official release of the Pokémon TCG!

---

## 📌 To-Do / Roadmap

* [ ] Add rarities and set numbers where missing
* [ ] Include card images / links (if permitted)
* [ ] Expand to other Scarlet & Violet expansions
* [ ] Provide CSV + SQLite versions for easier data manipulation

---

## 🤝 Contributing

Contributions are welcome!
If you’d like to help by:

* Fixing data errors
* Adding new sets
* Improving formatting

Please open an **Issue** or submit a **Pull Request**.

---

## 📜 License

This project is released under the **MIT License**.
---

Would you like me to **make the README more “data-science” focused** (emphasizing how researchers can use it for NLP/ML), or more **collector/player focused** (emphasizing deckbuilding and TCG use)?
