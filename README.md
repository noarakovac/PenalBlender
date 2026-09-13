# 3D Animacija penala

> Kratka animacija u Blenderu koja prikazuje 3D model lika kako izvodi nogometni penal (šutira loptu u gol).

## 📌 Opis projekta

Projekt je izrađen u sklopu kolegija 3D računalna grafika na Fakultetu primjenjene matematike i informatike Osijek. Cilj projekta bio je izraditi 3D model lika, pripremiti ga za animaciju (rigging) te izraditi kratku animiranu scenu u kojoj lik izvodi udarac na penal.

Animacija prikazuje:
- postavljanje lika i lopte na scenu,
- zalet i udarac lika prema lopti,
- putanju lopte prema golu.

## 🎯 Glavne funkcionalnosti / značajke

- Ručno modeliran 3D lik u Blenderu (low-poly pristup)
- Izrada i dodjela materijala (MTL) liku
- Rigging / kostur lika za potrebe animacije 
- Keyframe animacija pokreta udarca (šuta) na penal
- Kamera i osvjetljenje scene prilagođeni prikazu udarca
- Render animacije i izvoz gotovog videa

## 🛠️ Korišteni alati

- **Blender 5.0.1** – modeliranje, rigging, animacija, render
- Format izvoza modela: `.obj` / `.mtl`

## 📁 Struktura repozitorija

```
├── README.md
├── blend/
│   └── projekt.blend        # glavna Blender scena s animacijom
├── model/
│   ├── char.obj              # eksportirani model lika
│   └── char.mtl              # materijali modela
├── render/                   # (opcionalno) render slike / video isječci
└── docs/
    └── seminarski_rad.pdf    # seminarski rad o projektu
```

## ▶️ Kako otvoriti / pokrenuti projekt

1. Preuzmite ili klonirajte repozitorij:
   ```
   git clone [URL repozitorija]
   ```
2. Otvorite datoteku `projekt.blend` u Blenderu 
3. Za pregled animacije: pritisnite Space u Timeline prozoru ili pokrenite render animacije (`Render > Render Animation`).
4. Model lika bez animacije možete zasebno pregledati importom `char.obj` u bilo koji 3D alat koji podržava OBJ format.

## 🎬 Video animacije

📺 YouTube: **(https://www.youtube.com/watch?v=-XYryP_GU8o&t=2s)**

## ⚠️ Izazovi i rješenja (kratko, detaljno u seminarskom radu)

- Problem s deformacijom mreže tijekom animacije udarca – riješeno dodatnim weight paintingom
- Sinkronizacija pokreta noge i lopte – riješeno ključnim točkama (keyframes) usklađenim s fizikom leta lopte

## 👤 Autor

- **Noa Rakovac** – 3D računalna grafika, 2025/2026
