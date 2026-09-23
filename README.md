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

### 📅 Heti Mérföldkövek és Célkitűzések

- [ ] **1. hét: Projektindítás és Adatfeltárás**
  - Repó és környezet beállítása (Git, Jupyter, Python csomagok).
  - Adathalmaz letöltése és beolvasása `pandas`-szal.
  - Alapvető struktúra áttekintése (`shape`, adattípusok, oszlopok listája).
  - Modellezési cél definiálása (pl. étrend klasszifikációja méret és kor alapján).

- [ ] **2. hét: Felfedező Adatelemzés (EDA) és Vizualizáció**
  - Oszloponkénti eloszlások ábrázolása (hisztogramok, KDE görbék a méretekre).
  - Kategóriás változók (étrend, típus, korszak) gyakorisági oszlopdiagramjai.
  - Korrelációs mátrix és hőtérkép készítése `seaborn`-nal.
  - Ábrák alatti tanulságok megfogalmazása szöveges cellákban.

- [ ] **3. hét: Adattisztítás és Feature Engineering**
  - Hiányzó adatok (NaN értékek) feltárása és kezelése (törlés vagy imputálás).
  - Kiugró értékek (outlierek) vizsgálata boxplotokkal és szűrése.
  - Kategóriás változók kódolása gépi tanuláshoz (One-Hot Encoding).
  - Új változó származtatása (pl. faj létezési időtartama: `max_ma - min_ma`).
  - Adatok bontása tanító és teszt halmazra (`train_test_split`).

- [ ] **4. hét: Hipotézisvizsgálat és Modellezés**
  - Statisztikai hipotézis felállítása és tesztelése (pl. kétmintás t-próba a méretekre).
  - Baseline modell illesztése és tanítása (pl. Logisztikus regresszió).
  - Összetettebb modellek illesztése (pl. Döntési fa, Random Forest).
  - Hiperparaméter-hangolás alapjai.

- [ ] **5. hét: Eredmények kiértékelése és összehasonlítása**
  - Modellek tesztelése a teszthalmazon (Accuracy, Precision, Recall, F1-score).
  - Tévesztési mátrix (Confusion Matrix) megjelenítése hőtérképpel.
  - Modellek összehasonlító táblázatának és grafikonjának elkészítése.
  - Változók fontosságának vizsgálata (`feature_importances_`).

- [ ] **6. hét: Összegzés és felkészülés a bemutatásra**
  - Teljes notebook újrafuttatása hiba nélkül (*Restart & Run All*).
  - Kódkommentek és szöveges magyarázatok véglegesítése.
  - Rövid (5-10 perces) diasor vagy jegyzet vázlat elkészítése a bemutatóra.

---


## 📂 Mappaszerkezet

```text
├── data/
│   └── dinosaurs.csv           # A felhasznált nyers adathalmaz
├── dino_projekt.ipynb          # Dokumentált, diagramokkal illusztrált Jupyter Notebook
├── README.md                   # Projekt dokumentáció
└── requirements.txt            # Szükséges Python csomagok
