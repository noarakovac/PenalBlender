# 3D Animacija: Penal (Blender)

**Autor:** Noa Rakovac


## 🥅 Pregled

Ovaj repozitorij sadrži 3D animaciju izrađenu u **Blenderu**, u sklopu kolegija **3D računalna grafika**. Projekt prikazuje low-poly 3D lika u dresu hrvatske nogometne reprezentacije koji izvodi udarac na nogometni penal, a zatim slavi pogodak.

Animacija (1920×1080, 24 fps, 210 sličica / 8.75 s, ukupno 210 keyframeova) montirana je kroz više kutova snimanja: širi kadar terena, krupni plan zaleta i udarca, krupni plan lopte kraj grede, ptičja perspektiva proslave pogotka te završni krupni plan gola.

Cilj projekta bio je kroz cijeli produkcijski proces (modeliranje, materijali, rigging, animacija, montaža, render) primijeniti tehnike računalne grafike obrađene na kolegiju.


---

## 🚀 Značajke

- Ručno modeliran **3D lik** u Blenderu (low-poly pristup); dres hrvatske nogometne reprezentacije ručno je obojan po plohama, prema pronađenoj referentnoj slici (svaka ploha mreže ima vlastitu boju, bez teksture)
- **Rigging** lika izrađen pomoću alata Mixamo (auto-rigging); ključne poze noge koja izvodi udarac postavljene su ručno u Blenderu, rotacijom kostiju (interpolacija: Ease)
- **Dvije zasebne keyframe animacije**: udarac na penal (zalet, zamah, kontakt s loptom) i proslava pogotka (gotova animacija iz Mixamove knjižnice)
- **Promjena kutova kamere kroz Constant interpolaciju** — kamera "skoči" na sljedeću poziciju bez glatkog prijelaza, čime nastaje efekt reza (cut) bez potrebe za više zasebnih kamera
- Pozadina scene prikazana i osvijetljena pomoću **HDRI teksture** ("Lilienstein", Poly Haven)
- Finalni **render** cijele animirane scene (1920×1080, 24 fps)

---

## 📦 Kako koristiti repozitorij

### 1. Kloniranje repozitorija

```
git clone https://github.com/noarakovac/PenalBlender.git
cd PenalBlender
```

### 2. Struktura projekta

Nakon kloniranja, struktura mapa izgleda ovako:

```
PenalBlender/
├── blender_file/         # Glavna Blender (.blend) datoteka s animacijom
├── model_export/         # Model lika eksportiran kao .obj / .mtl
├── renders/               # Finalni render (video) i isječci animacije
├── presentation/          # PowerPoint prezentacija projekta
├── seminarski_rad/        # Seminarski rad (Word/PDF) o projektu
├── README.md              # Dokumentacija projekta
```

### 3. Otvaranje i pregled animacije

- Otvorite `.blend` datoteku iz mape `blender_file/` u Blenderu 
- Za pregled animacije pritisnite razmaknicu (Space) u Timeline/Dope Sheet prozoru
- Za render pritisnite `Ctrl+F12` (Render Animation) ili `F12` za pojedinačni kadar

### 4. Pregled modela bez animacije

- Model lika (`char.obj` / `char.mtl`) iz mape `model_export/` možete zasebno učitati u bilo koji alat koji podržava OBJ format

### 5. Pregled prezentacije

- Mapa `presentation/` sadrži PowerPoint prezentaciju projekta korištenu za izlaganje

---

## 🛠 Metodologija

- Naučene tehnike Blendera primijenjene kroz praktičnu izradu projekta
- Modeliranje 3D lika prilagođeno za animaciju (low-poly, jedinstvena mreža)
- Postavljanje kostura (armature) pomoću alata Mixamo (auto-rigging)
- Ključne poze noge za udarac postavljene ručno u Blenderu (forward kinematics, interpolacija Ease), uz resetiranje poze prije svake sljedeće
- Proslava pogotka animirana je primjenom gotove animacije iz Mixamove knjižnice na kostur vlastitog modela
- Rezovi između kutova kamere postignuti Constant interpolacijom ključnih kadrova kamere
- Pozadina (nebo/šuma) prikazana i osvijetljena pomoću HDRI teksture

---

## 🔗 Resursi i reference

- 📘 Blender dokumentacija: [docs.blender.org](https://docs.blender.org/)
- 📹 *Creating Stylized Low Poly Characters in Blender* — YouTube, [youtube.com/watch?v=-XYryP_GU8o](https://www.youtube.com/watch?v=-XYryP_GU8o) (polazište za oblik/geometriju modela lika)
- 🦴 [Mixamo](https://www.mixamo.com/) (Adobe) — auto-rigging kostura i animacija proslave pogotka
- 🌄 [Poly Haven — "Lilienstein"](https://polyhaven.com/a/lilienstein) — HDRI tekstura za pozadinu i osvjetljenje
- 3d računalna grafika – materijali s predavanja i vježbi

---

## 🔮 Moguća poboljšanja

Uz više vremena, projekt bi se mogao unaprijediti kroz:

- Fizikalnu simulaciju lopte (**Rigid Body**) umjesto ručnih keyframeova
- Detaljniju teksturu lika, trave i stadiona
- Dodatne kutove kamere i dodatne animacije (npr. reakcija publike)

---

## 📬 Kontakt

Za pitanja ili prijedloge:
**Noa Rakovac** – student, MiR program (Sveučilište Josipa Jurja Strossmayera in Osijek)
E-mail: noa.rakovac@gmail.com · Slobodno otvorite issue na repozitoriju.
