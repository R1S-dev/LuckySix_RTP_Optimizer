# 🎯 LuckySix_RTP_Optimizer

Ovaj projekat predstavlja simulaciju igre brojeva inspirisanu konceptom "Lucky Six", uz analizu RTP-a (*Return to Player*) i optimizaciju izvučenih brojeva pomoću heurističkog algoritma (AI). Cilj je da se balansira isplativost igre tako da RTP ostane blizu unapred definisane vrednosti.

---

## 🎯 Ciljevi projekta

- Simulacija hiljada tiketa koje generišu igrači sa nasumičnim brojevima.
- Računanje RTP-a na osnovu ukupne isplate i ukupnog uloga.
- Implementacija AI algoritma za "štelovanje" brojeva u cilju dostizanja željenog RTP-a.
- Upoređivanje dva modela:
  - 📘 Bez snage tiketa (svi tiketi imaju istu vrednost)
  - 📗 Sa snagom tiketa (različita uplata po tiketu – ponderisani uticaj)

---

## ⚙️ Korišćene tehnologije

- Python 3.x
- `matplotlib` – za prikaz grafova
- `random`, `collections.Counter` – za generisanje i analizu brojeva

---

## 🧠 Strategija optimizacije (AI)

- Inicijalno izvlačenje 35 brojeva iz opsega (1–48).
- Iterativno menjanje mesta brojevima (zamena 2 nasumična broja).
- Računanje novog RTP-a; ako se približava ciljanom – prihvata se nova kombinacija.
- Zaustavljanje kada je odstupanje manje od zadate tolerancije ili nakon maksimalnog broja iteracija.

---

## 📈 Vizualizacija

Na kraju simulacije prikazuje se graf koji poredi:
- 📘 Model bez snage tiketa (fiksna uplata)
- 📗 Model sa nasumičnim ulogom (realna snaga tiketa)
- 🔴 Crvena linija – ciljani RTP
