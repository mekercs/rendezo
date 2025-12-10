# rendezo 🗂️

## Rövid leírás  
A **rendezo** egy egyszerű Python alapú mappa-rendező program, amely automatikusan almappákba sorolja a fájlokat a kiterjesztésük alapján. A célja, hogy gyorsan és hatékonyan rendet tegyen például a letöltések mappádban vagy bármilyen rendezetlen könyvtárban.

## ⚙️ Miért hasznos?
- Automatikusan rendszerezi a fájlokat típus szerint  
- Létrehozza a szükséges almappákat  
- Egyszerűen használható: csak kiválasztod a mappát, a program pedig elvégzi a munkát  
- Minimális függőség: csak Python és a beépített `tkinter`

## 📝 Hogyan működik?
A program bekér egy mappát, majd végignézi az ott található fájlokat.  
A kiterjesztés alapján az előre definiált kategóriák szerint külön almappákba helyezi őket.  
Ezeket az almappákat automatikusan létrehozza, ha még nem léteznek.

A fájlokat a következő logika alapján kezeli például:
- Dokumentumok (`pdf`, `docx`, `txt` stb.)  
- Képek (`jpg`, `png`, `gif`)  
- Videók (`mp4`, `avi`)  
- Zenék (`mp3`, `wav`)  
- Python fájlok (`py`)  
és így tovább — ezek a `anyaaa` szótárban szabadon módosíthatók.

## 🚀 Telepítés és futtatás

1. Győződj meg róla, hogy Python 3 telepítve van.
2. Klónozd a repót:
   ```bash
   git clone https://github.com/mekercs/rendezo.git
Lépj be a mappába és futtasd:

bash
Kód másolása
cd rendezo
python rendező.py
Válaszd ki a rendezendő mappát, és készen is van.

🛠️ Testreszabás
A anyaaa szótárban saját igényeid szerint módosíthatod:

hogy mely kiterjesztések melyik mappába kerüljenek,

a mappák elnevezését.

⚠️ Fontos
A program csak a kiválasztott mappa felső szintjén lévő fájlokat rendezi.

Almappákat nem dolgoz fel.

Ha fontos fájlokat rendezel, először próbáld ki egy kis tesztmappával.

👤 Készítette
mekercs
