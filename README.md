# dino-project
Adattudományi projektmunka dinoszaurusz leletek feltáró elemzésére (EDA), hipotézisvizsgálatára és gépi tanulási modellezésére.

# 🦖 Dinoszaurusz Adathalmaz Elemzés és Modellezés

Projektmunka a **Bevezetés az adattudományokba** tantárgy keretében.

A projekt célja a paleontológiai leletekből származó dinoszaurusz adatok feltáró elemzése (EDA), statisztikai összefüggéseinek vizsgálata, valamint felügyelt gépi tanulási modellek építése és összehasonlítása.

---

## 📌 A Projekt Célkitűzései és Problémafelvetés
- **Feltáró adatelemzés (EDA):** Dinoszauruszok fizikai tulajdonságainak (méret, mozgásforma), földtörténeti korszakainak és elterjedési területeinek vizsgálata és vizualizációja.
- **Hipotézisvizsgálat:** Statisztikai összefüggések ellenőrzése a korszakok és a testméretek között (pl. a jura és kréta kori ragadozók méretkülönbségei).
- **Modellezés (Gépi tanulás):** 
  - Osztályozási feladat (pl. étrend előrejelzése morfológiai és földrajzi adatok alapján) vagy regressziós feladat (testhossz becslése).
  - Alapmodell (Baseline) és összetettebb modellek (pl. Döntési fa, Random Forest) teljesítményének összevetése teszthalmazon.

---

## 📊 Adatforrás

A projektben felhasznált adatok a Kaggle-ről származnak:
* **Forrás:** [Dinosaur Dataset by Smruthi](https://www.kaggle.com/datasets/smruthiiii/dinosaur-dataset)
* **Primer forrás:** [The Paleobiology Database (PBDB)](https://paleobiodb.org/)
* **Licenc / Hozzáférés:** Nyílt hozzáférésű adatbázis tudományos és oktatási célokra.

---

## 📂 Mappaszerkezet

```text
├── data/
│   └── dinosaurs.csv           # A felhasznált nyers adathalmaz
├── dino_projekt.ipynb          # Dokumentált, diagramokkal illusztrált Jupyter Notebook
├── README.md                   # Projekt dokumentáció
└── requirements.txt            # Szükséges Python csomagok
